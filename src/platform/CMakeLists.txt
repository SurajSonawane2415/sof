# SPDX-License-Identifier: BSD-3-Clause

if(CONFIG_LIBRARY)
	add_subdirectory(library)
	return()
endif()

if(CONFIG_TIGERLAKE)
	add_subdirectory(tigerlake)
elseif(CONFIG_IMX8 OR CONFIG_IMX8X)
	add_subdirectory(imx8)
elseif(CONFIG_IMX8M)
	add_subdirectory(imx8m)
elseif(CONFIG_IMX8ULP)
	add_subdirectory(imx8ulp)
elseif(CONFIG_AMD)
	add_subdirectory(amd)
elseif(CONFIG_MT8186)
	add_subdirectory(mt8186)
elseif(CONFIG_MT8188)
	add_subdirectory(mt8188)
elseif(CONFIG_MT8195)
        add_subdirectory(mt8195)
elseif(CONFIG_MT8196)
        add_subdirectory(mt8196)
elseif(CONFIG_MT8365)
	add_subdirectory(mt8365)
endif()
