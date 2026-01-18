set(MI_PLUGIN_PREFIX "integrators")

add_plugin(aov        aov.cpp)
add_plugin(depth      depth.cpp)
add_plugin(direct     direct.cpp)
add_plugin(moment     moment.cpp)
add_plugin(manifold_path_guiding
           MPG/manifold_path_guiding.cpp
           MPG/manifold_path_guiding.h
           MPG/ann.h
           MPG/chain_distribution.h
           MPG/dtree.h
           MPG/spatial_structure.h
           MPG/util.h)
add_plugin(path       path.cpp)
add_plugin(ptracer    ptracer.cpp)
add_plugin(stokes     stokes.cpp)
add_plugin(volpath    volpath.cpp)
add_plugin(volpathmis volpathmis.cpp)

set(MI_PLUGIN_TARGETS "${MI_PLUGIN_TARGETS}" PARENT_SCOPE)
