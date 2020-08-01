set(defines "")
if(MSVC)
  list(APPEND defines _CRT_SECURE_NO_WARNINGS)
endif()

Ubpa_AddTarget(
  MODE INTERFACE
  INC
    "${PROJECT_SOURCE_DIR}/include"
  DEFINE
    RAPIDJSON_HAS_STDSTRING
	${defines}
)
