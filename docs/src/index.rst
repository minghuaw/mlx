MLX
===

MLX is a NumPy-like array framework designed for efficient and flexible machine
learning on Apple silicon, brought to you by Apple machine learning research.

The Python API closely follows NumPy with a few exceptions. MLX also has a
fully featured C++ API which closely follows the Python API.

The main differences between MLX and NumPy are:

 - **Composable function transformations**: MLX has composable function
   transformations for automatic differentiation, automatic vectorization,
   and computation graph optimization.
 - **Lazy computation**: Computations in MLX are lazy. Arrays are only
   materialized when needed.
 - **Multi-device**: Operations can run on any of the supported devices (CPU,
   GPU, ...)

The design of MLX is inspired by frameworks like `PyTorch
<https://pytorch.org/>`_, `Jax <https://github.com/google/jax>`_, and
`ArrayFire <https://arrayfire.org/>`_. A notable difference from these
frameworks and MLX is the *unified memory model*. Arrays in MLX live in shared
memory. Operations on MLX arrays can be performed on any of the supported
device types without performing data copies. Currently supported device types
are the CPU and GPU.

.. toctree::
   :caption: Install
   :maxdepth: 1

   install

.. toctree::
   :caption: Usage 
   :maxdepth: 1

   usage/quick_start
   usage/lazy_evaluation
   usage/unified_memory
   usage/indexing
   usage/saving_and_loading
   usage/function_transforms
   usage/compile
   usage/numpy
   usage/distributed
   usage/using_streams
   usage/export

.. toctree::
   :caption: Examples
   :maxdepth: 1

   examples/linear_regression
   examples/mlp
   examples/llama-inference

.. toctree::
   :caption: Python API Reference
   :maxdepth: 1

   python/array
   python/data_types
   python/devices_and_streams
   python/export
   python/ops
   python/random
   python/transforms
   python/fast
   python/fft
   python/linalg
   python/metal
   python/memory_management
   python/nn
   python/optimizers
   python/distributed
   python/tree_utils

.. toctree::
   :caption: C++ API Reference
   :maxdepth: 1

   cpp/ops

.. toctree::
   :caption: Further Reading
   :maxdepth: 1

   dev/extensions
   dev/metal_debugger
   dev/custom_metal_kernels
   dev/mlx_in_cpp
