# Copyright (c) 2018 Cisco and/or its affiliates.
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at:
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

add_vpp_plugin(vmxnet3
  SOURCES
  cli.c
  format.c
  input.c
  output.c
  plugin.c
  vmxnet3.c
  vmxnet3_api.c

  MULTIARCH_SOURCES
  input.c
  output.c

  API_FILES
  vmxnet3.api

  API_TEST_SOURCES
  vmxnet3_test.c

  INSTALL_HEADERS
  vmxnet3_all_api_h.h
  vmxnet3_msg_enum.h
)
