include_directories(..)

set(DEQP_VK_CLIPPING_SRCS
	vktClippingTests.cpp
	vktClippingTests.hpp
	vktClippingUtil.cpp
	vktClippingUtil.hpp
	)

set(DEQP_VK_CLIPPING_LIBS
	tcutil
	vkutil
	)

add_library(deqp-vk-clipping STATIC ${DEQP_VK_CLIPPING_SRCS})
target_link_libraries(deqp-vk-clipping ${DEQP_VK_CLIPPING_LIBS})
