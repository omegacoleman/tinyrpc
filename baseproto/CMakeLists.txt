﻿PROTOBUF_GENERATE_CPP(PROTO_RPC_SERVICE_PTL_SRC PROTO_RPC_SERVICE_PTL_HDRS rpc_service_ptl.proto)

add_custom_target(baseproto_gen ALL DEPENDS rpc_service_ptl.proto SOURCES ${PROTO_RPC_SERVICE_PTL_SRC} ${PROTO_RPC_SERVICE_PTL_HDRS})
