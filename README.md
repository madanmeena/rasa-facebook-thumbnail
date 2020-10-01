# rasa-facebook-thumbnail

## SHELL
docker run  --user $(id -u):$(id -g) -it -v $(pwd):/app --entrypoint rasa rasa/rasa:1.10.12-full shell  --debug
## TRAIN
docker run  --user $(id -u):$(id -g) -it -v $(pwd):/app --entrypoint rasa rasa/rasa:1.10.12-full train  --debug
## ACTION
docker run -v $(pwd):/app rasa/rasa:1.10.12-full run actions --port 5006 --debug
## RUN
docker run  --user $(id -u):$(id -g) -it -v $(pwd):/app --entrypoint rasa rasa/rasa:1.10.12-full run  --debug