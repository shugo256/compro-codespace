# https://mcr.microsoft.com/v2/vscode/devcontainers/cpp/tags/list
FROM mcr.microsoft.com/devcontainers/cpp:ubuntu-22.04

# [Optional] Uncomment this section to install additional vcpkg ports.
# RUN su vscode -c "${VCPKG_ROOT}/vcpkg install <your-port-name-here>"

RUN apt-get update && DEBIAN_FRONTEND=noninteractive \
    && apt-get install -y --no-install-recommends \
    python3-pip

# online-judge-tools: https://pypi.org/project/online-judge-tools
RUN pip3 install --break-system-packages \
    online-judge-tools \
    online-judge-template-generator
