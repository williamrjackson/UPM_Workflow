# UPM_Workflow
Testing UPM Post-Commit autoversioning workflow

## The Plan

1. Trigger on [push] (to master only?)
2. Read package.json `"version"` value
3. If unchanged from previous (how do you know previous?), increment revision (eg x.y.{z+1})
4. If changed and > previous, use what's there
5. Tag revision as `v1`, `v1.0`, & `v1.0.0`
6. Update readme with Install Instructions, providing link with target `#vX.Y.Z`

## The Aforementioned Installation Instructions

- In Unity, go to `Window` > `Package Manager`
- Click the plus and select `Add package from git URL`
- Paste:
 `https://github.com/williamrjackson/UPM_Workflow.git#v1.0`
 OR
 `https://github.com/williamrjackson/UPM_Workflow.git#v1.0.11`
- Click "Add"
- Optionally install examples

Here's a line to modify as a meaningless commit/push to trigger.
