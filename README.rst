StereoVision: Library and utilities for 3d reconstruction from stereo cameras
=============================================================================

StereoVision is a package for working with stereo cameras, especially with the
intent of using them to produce 3D point clouds. The focus is on performance,
ease of usability, and the ability to construct 3D imaging setups cheaply.

StereoVision relies heavily on OpenCV. If you're not sure about what a given
variable does or what values would make sense for it and no explanation is
provided in the StereoVision documentation, refer to OpenCV's documentation in
order to better understand how they work.

It's available on PyPI, so you can install it like this::

    pip install StereoVision

If you find a bug or would like to request a feature, please `report it with
the issue tracker <https://github.com/erget/StereoVision/issues>`_. If you'd
like to contribute to StereoVision, feel free to `fork it on GitHub
<https://github.com/erget/StereoVision>`_.

StereoVision is released under the GNU General Public License, so feel free to
use it any way you like. It would be nice to let me know if you do anything
cool with it though.

Author: `Daniel Lee <Lee.Daniel.1986@gmail.com>`_

NASGR Fork
----------

I will be working to add integration with pcl. 

I'll add output to pcl data formats in images_to_pointcloud, as well as the PCD file format

First, I'll need to link the cpp pcl library to python or vice versa, because the current python-pcl library 
does not support colors, or adding points, and is relatively new. The AUVSI competition requires
color recognition.

I could add on to the python-pcl library, but it will be simpler to embed python in cpp for now.
