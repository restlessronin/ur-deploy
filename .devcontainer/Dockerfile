FROM restlessronin/foundry AS foundry

FROM mcr.microsoft.com/devcontainers/typescript-node:0-18 AS node

COPY --from=foundry /usr/local/bin/forge /usr/local/bin/forge
COPY --from=foundry /usr/local/bin/cast /usr/local/bin/cast
COPY --from=foundry /usr/local/bin/anvil /usr/local/bin/anvil

WORKDIR /workspaces
