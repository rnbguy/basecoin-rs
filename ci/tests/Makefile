all: create-channel token-transfer upgrade-client

create-channel:
	@echo "Creating channel..."
	bash create-channel.sh
	@echo "Channel created"

upgrade-client: token-transfer
	@echo "Upgrading client..."
	bash upgrade-client.sh
	@echo "Client upgraded"

token-transfer: create-channel
	@echo "Transferring tokens..."
	bash token-transfer.sh
	@echo "Tokens transferred"

.PHONY: create-channel token-transfer upgrade-client
