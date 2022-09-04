proto:
	protoc --proto_path=pkg --go_out=pkg \
		--go_opt=paths=source_relative \
		--go-grpc_out=require_unimplemented_servers=false:pkg \
		--go-grpc_opt=paths=source_relative \
		pkg/**/pb/*.proto

server:
	go run main.go