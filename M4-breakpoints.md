# M4 Breakpoint Investigation

## Evidence-based decision

The original stylesheet used a media query at `max-width: 600px`. Testing did not show a specific layout problem that began at 600px. At 600px, the navigation, table, and contact form remained usable. The first clear navigation problem appeared at 320px, where the links wrapped onto a second line.

After the navigation spacing was revised, the navigation was retested at 320px, 768px, and 1440px. The links stayed in one row at all three widths.

Therefore, the 600px breakpoint does not have direct observable support from the recorded tests. Future breakpoint decisions should be based on the first width where the content becomes difficult to use, rather than on a commonly chosen screen width.

## Testing limitations

The nearby widths 576px, 599px, 600px, and 640px were not tested individually. They should not be described as measured results. The conclusion above is limited to the widths that were actually observed and recorded.

## Breakpoint challenge evidence

The QA challenge asked whether the 600px breakpoint could be defended without inventing an unobserved symptom. The conclusion was that no direct observable support was found for 600px, while the first clear issue appeared at 320px. The final AI exchange was saved in `M4-screens/breakpoint-challenge-final.png`.
