---
-api-id: P:Windows.Perception.Spatial.Surfaces.SpatialSurfaceMesh.CoordinateSystem
-api-type: winrt property
---

<!-- Property syntax
public Windows.Perception.Spatial.SpatialCoordinateSystem CoordinateSystem { get; }
-->

# Windows.Perception.Spatial.Surfaces.SpatialSurfaceMesh.CoordinateSystem

## -description
Gets the coordinate system in which the VertexPositions and VertexNormals buffers express their coordinates.

## -property-value
The vertex coordinate system.

## -remarks
Unlike other spatial data structures, vertex buffers and normal buffers are quite heavy, and it would be prohibitive to update all of their coordinates every frame. Instead, appscan transfer these buffers to the GPU or process them for physics once, and then reason about how the surface's SpatialCoordinateSystem then changes its relative transform to the app's other relevant coordinate systems in future frames.

## -examples

## -see-also
