# skeletonization
Automatically exported from code.google.com/p/skeletonization

Because the code uses a KdTree Package which only supports 32-bit platform, you can replace parts of the functions that use kdTree with other non-KdTree functions on your 64-bit platform. For example, the KdTree KNN function can be replaced by findNearestNeighbors() of pointCloud structure; The ball query function can be replaced by the Rangesearch () function. After all the related functions are replaced, you can delete the kdtree_build and kdtree_delete so that the program could be available on 64-bit platform.
