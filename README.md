GDM_CLASS: an implementation of the Generalized Dark Matter model in the Cosmic Linear Anisotropy Solving System
================================================================================================================

**Original CLASS authors**: Julien Lesgourgues and Thomas Tram

**GDM implementation authors**: Stéphane Ilic, Michael Kopp, Daniel B. Thomas, Constantinos Skordis


Compiling GDM_CLASS and getting started
---------------------------------------

The process of compiling and running GDM_CLASS is strictly identical to the original CLASS code. Please refer to the CLASS code [webpage](http://class-code.net) and [GitHub repository](https://github.com/lesgourg/class_public) for detailed instructions.


Generalized Dark Matter model implementation
--------------------------------------------

GDM_CLASS is a modification of the CLASS code which adds the phenomenologically motivated Generalized Dark Matter (GDM) model from [Hu (1998)](https://arxiv.org/abs/astro-ph/9801234). A detailed investigation of the theoretical aspects related to this model can be found in the [following article](https://arxiv.org/abs/1605.00649).

The GDM model relaxes the assumptions about the pressureless nature of cold dark matter, and allows for non-zero sound speed and viscosity. The current implementation of the GDM model in GDM_CLASS allows the user to provide any choice for those three additional degree of freedom, in the form of three (smooth) binned functions: the equation of state, the sound speed, and the viscosity of the GDM fluid as a function of scale factor. The binning in time is entirely customizable by the user.

A thorough description of the CLASS code parameters is available in the ``explanatory.ini`` file. All additional parameters introduced in GDM_CLASS are described in a separate file, ``GDM.ini``.


Python wrapper
--------------

Similarly to the original CLASS code, a Python wrapper is included in GDM_CLASS which is automatically compiled and installed at the same time as the main code (provided you use the ``make`` command and not simply the ``make class`` one). Since no modification were done to this wrapper, we also refer to the [official CLASS documentation](https://github.com/lesgourg/class_public/wiki) for details on the wrapper and its compilation.


Developing the code
--------------------

Participation to the further development of the code is welcome. Feel free to clone the current repository, develop your own branch, and get it merged to the public distribution. You may as well [open issues](https://github.com/s-ilic/gdm_class_public/issues) to discuss what new features you would like to see implemented.


Using the code
--------------

While CLASS is free to use, its authors request that publications using their code should cite at least the paper ["CLASS II: Approximation schemes"](http://arxiv.org/abs/1104.2933). Additionally, we have a similar request to the users of our modified code, and ask them to cite the following paper: `TBD-TBD-TBD`.


Support
-------

To get support related to the main CLASS code, please open a new issue on the [original CLASS repository](https://github.com/lesgourg/class_public). For an issue related to the GDM implementation, please [open an issue](https://github.com/s-ilic/gdm_class_public/issues) in the present repository.
