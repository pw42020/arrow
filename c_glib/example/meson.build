# -*- indent-tabs-mode: nil -*-
#
# Licensed to the Apache Software Foundation (ASF) under one
# or more contributor license agreements.  See the NOTICE file
# distributed with this work for additional information
# regarding copyright ownership.  The ASF licenses this file
# to you under the Apache License, Version 2.0 (the
# "License"); you may not use this file except in compliance
# with the License.  You may obtain a copy of the License at
#
#   http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing,
# software distributed under the License is distributed on an
# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
# KIND, either express or implied.  See the License for the
# specific language governing permissions and limitations
# under the License.

executable('build', 'build.c', dependencies: [arrow_glib], link_language: 'c')
executable(
    'extension-type',
    'extension-type.c',
    dependencies: [arrow_glib],
    link_language: 'c',
)
executable(
    'read-file',
    'read-file.c',
    dependencies: [arrow_glib],
    link_language: 'c',
)
executable(
    'read-stream',
    'read-stream.c',
    dependencies: [arrow_glib],
    link_language: 'c',
)
executable(
    'receive-network',
    'receive-network.c',
    dependencies: [arrow_glib],
    link_language: 'c',
)
executable(
    'send-network',
    'send-network.c',
    dependencies: [arrow_glib],
    link_language: 'c',
)

install_data(
    'README.md',
    'build.c',
    'extension-type.c',
    'read-file.c',
    'read-stream.c',
    'receive-network.c',
    'send-network.c',
    install_dir: join_paths(data_dir, meson.project_name(), 'example'),
)

subdir('lua')
subdir('vala')
