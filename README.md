# standalone-storybook-bug

**Steps to reproduce:**

1. `yarn`
1. `yarn serve-standalone-storybook`
1. `yarn storybook` (sets `--preview-url`)
1. Navigate to http://localhost:6006/
1. Observe that the `path` query param was no automatically applied
1. Click on any of the addon toolbar button, e.g., the outlines button.
1. Observe that the iframe now appears blank

**Additional notes:**

If you instead navigate to http://localhost:6006/?path= (`path` param intentionally left blank) then the Storybook behaves as expected.
