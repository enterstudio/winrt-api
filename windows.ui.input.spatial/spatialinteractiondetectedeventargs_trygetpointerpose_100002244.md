---
-api-id: M:Windows.UI.Input.Spatial.SpatialInteractionDetectedEventArgs.TryGetPointerPose(Windows.Perception.Spatial.SpatialCoordinateSystem)
-api-type: winrt method
---

<!-- Method syntax
public Windows.UI.Input.Spatial.SpatialPointerPose TryGetPointerPose(Windows.Perception.Spatial.SpatialCoordinateSystem coordinateSystem)
-->

# Windows.UI.Input.Spatial.SpatialInteractionDetectedEventArgs.TryGetPointerPose

## -description
Gets the user's gaze for use in routing this interaction to a SpatialGestureRecognizer.

On HoloLens, interactions should generally derive their targeting from the user's gaze, rather than trying to render or interact at the hand's location directly. Once an interaction has started, relative motions of the hand may be used to control the gesture, as with the Manipulation or Navigation gesture.

This method will return null if the specified coordinate system cannot be located at the moment.

## -parameters
### -param coordinateSystem
The coordinate system in which to express the gaze.

## -returns
The gaze.

## -remarks

## -examples

## -see-also
