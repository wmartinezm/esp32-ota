#set(COMPONENT_SRCS "main.c". 
#                   "wifi.c")
#set(COMPONENT_ADD_INCLUDEDIRS ".")
# Embed the server root certificate into the final binary
#set(COMPONENT_EMBED_TXTFILES ${IDF_PROJECT_PATH}/server_certs/ca_cert.pem)

idf_component_register(SRCS "main.c" "wifi.c"
                    INCLUDE_DIRS "."
                    EMBED_TXTFILES ${project_dir}/Server_Certs/ca_cert.pem)
#register_component()
