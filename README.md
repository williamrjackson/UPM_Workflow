# UPM_Workflow
Testing UPM Post-Commit autoversioning workflow

## The Plan

1. Trigger on push
2. Read package.json `"version"` value
3. If unchanged from previous (how do you know previous?), increment revision (eg x.y.{z+1})
4. If changed and > previous, use what's there
5. Tag revision as `v1`, `v1.0`, & `v1.0.0`
6. Update readme with install instructions providing link with target `#v1.0`
