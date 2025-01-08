# Accessibility Issue: Inconsistent Focus Styles

This repository demonstrates an accessibility issue related to the inconsistent support of the CSS `:focus-visible` pseudo-class in older browsers.  The issue occurs because the focus styles are only applied when the focus is visible, potentially leaving users with no visual indication of the currently active element.

## Problem

The `:focus-visible` pseudo-class is a relatively new addition to CSS and is not universally supported. Older browsers may not render elements styled with `:focus-visible`, resulting in inconsistent focus styles.  Users relying on keyboard navigation or assistive technologies will struggle to follow the interface's interaction flow.

## Solution

The recommended approach is to use a JavaScript polyfill or to create a fallback style that provides a consistent focus indicator, even for browsers that do not support `:focus-visible`.  The proposed solution uses a fallback style to ensure that an outline is always visible, improving accessibility for all users.