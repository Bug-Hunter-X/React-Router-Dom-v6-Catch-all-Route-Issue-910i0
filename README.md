# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a problem with the catch-all route (`path="/*"`) in React Router Dom v6.  The catch-all route should match any unmatched path, but this example shows it failing to do so under certain circumstances.

## Problem

The `path="/*"` route defined in the `App` component doesn't seem to intercept requests for paths not explicitly handled, even when there are no other exact path matches.  This should always be a final fallback.  The issue appears specific to the usage of v6.