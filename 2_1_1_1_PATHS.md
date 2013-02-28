# Path Variables

The following variables in this section described are ones which are related to:

* Querying where Theos stores certain resource files which may need to be referenced on a Makefile.
* Setting a path for Theos to store generated files during the build process.

## Theos Resource Locations

###### THEOS %C%
The path where Theos is located. As of recent Theos commits, is completely generated by Theos and ignores any previously set environment variable by the user.

Defined on *common.mk*.

###### THEOS\_MAKE_PATH %C%
The path where Theos' Makefiles are located. Save `common.mk`, Make inclusions should use this variable for defining locations of other Theos Makefiles to be included.

Defined on *common.mk*.

###### THEOS\_BIN_PATH %C%
The path where Theos stores its binaries, such as install, query and bootstrap scripts, Logos, NIC, and others.

Defined on *common.mk*.

###### THEOS\_LIBRARY_PATH %C%
The path where libraries which are to be meant for Theos use only are placed. It is automatically placed at the project's *library path* during the linking process.

Defined on *common.mk*.

###### THEOS\_INCLUDE_PATH %C%
The path where headers meant for use in Theos projects are stored. During compilations added to the *include path*.

Defined on *common.mk*.

###### THEOS\_MODULE_PATH %C%
The path where [Theos Modules](./6_0_MODULES.md) are stored.

Defined on *common.mk*.

## Project Build Locations

###### THEOS\_BUILD\_DIR %S%
The directory which houses a project's object directory, staging directory and built packages.

Defaults to the project's root directory.<br />
Defined on *common.mk*.


###### THEOS\_OBJ\_DIR\_NAME %S%
The name of the directory which houses a project's built object files and main executable.

Defaults to "obj".<br />
Defined on *common.mk*.

###### THEOS\_STAGING\_DIR %S%
The name of the project's [staging](./4_1_INVOKABLE.md#package) directory.
	
Defaults to "_".<br />
Defined on *common.mk*.