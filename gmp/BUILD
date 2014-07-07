[
{ "autoconf": {
    "name": "gmp_make",
    "configure_args": [ "--disable-assembly" ],
    "outs": [
       "$GEN_DIR/lib/libgmp.a"
     ],
    "licenses": [ "http://opensource.org/licenses/gpl-2.0",
                  "http://opensource.org/licenses/lgpl-3.0" ]
                  
  } },
  { "cc_library": {
     "name": "gmp",
     "cc_objects": [
          "$GEN_DIR/lib/libgmp.a"
     ],
     "strict_file_mode": false,
     "include_dirs": [ "." ],
     "dependencies": [ ":gmp_make" ],
     "env" : {
       "GMP_LIB" : "$GEN_DIR/lib",
       "GMP_INCLUDE" : "$SRC_DIR/include",
     }
  } }
]
]