# Implementation Plan - Refining Stays Section Heading

Make the "OUR STAYS" and "Find Your Perfect Retreat" heading section much larger and more impactful to fill the visual gap and feel premium.

## Proposed Changes

### [index.html](file:///c:/Users/chitr/Downloads/my%20websites/palm%20715/palm-715-jorhat-main/index.html)

#### [MODIFY] Styles (within `<style>` tag)
- **.rooms-section**: Increase `padding-top` to `80px`.
- **.section-label**: 
    - `font-size: 16px`
    - `letter-spacing: 0.25em`
    - `font-family: 'DM Sans', sans-serif`
    - `font-weight: 700`
    - `color: #1B4332`
    - `margin-bottom: 16px`
- **.section-title**: 
    - `font-size: clamp(56px, 8vw, 96px)`
    - `font-family: 'Cormorant Garamond', serif`
    - `font-weight: 800`
    - `line-height: 1.05`
    - `color: #1B4332`
    - `margin-bottom: 24px`
- **.section-title em**: Ensure it remains `color: #c9a84c` and italic.
- **New .section-subtitle**: 
    - `font-family: 'DM Sans', sans-serif`
    - `font-weight: 400`
    - `font-size: 18px`
    - `color: #6b7280`
    - `margin-bottom: 48px`
- **New .decorative-line**: 
    - `width: 80px`
    - `height: 2px`
    - `background: #c9a84c`
    - `margin: 16px auto 40px auto` (centered)

#### [MODIFY] HTML Markup (around line 2045)
- Update the `.section-header` container:
    ```html
    <div class="section-header center">
        <span class="section-label">OUR STAYS</span>
        <h2 class="section-title">Find Your Perfect <em>Retreat</em></h2>
        <div class="decorative-line"></div>
        <p class="section-subtitle">Three private rooms. One unforgettable stay.</p>
    </div>
    ```

## Verification Plan

### Manual Verification
- Open `index.html` in a browser.
- Verify the "OUR STAYS" label matches 16px, bold, and specific spacing.
- Verify the main heading uses `clamp` and feels very large and premium.
- Confirm the new subtitle and gold line are present and styled correctly.
- Verify `padding-top: 80px` for the section.
- Test responsiveness on mobile devices.
