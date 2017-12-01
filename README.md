# Kafka Autocomplete

This repository implements bash completion for some of the Kafka command line
utilities.

In order to build and install:

    git clone https://github.com/Landoop/kafka-autocomplete.git
    cd kafka-autocomplete
    ./build.sh

You will find the completion file under `release/kafka`. You can source it in
your terminal or drop it in `/etc/bash_completion.d/`. You have to set up
bash-completion too, which depends on your distribution of choice.

Currently completion is provided for five utilities:

- kafka-topics
- kafka-console-consumer / kafka-avro-console-consumer
- kafka-console-producer / kafka-avro-console-producer
- kafka-mirrormaker
- kafka-acls

We provide completion for options, kafka configs and kafka properties.
Especially for `kafka-topics` if you set the `--zookeeper` switch, we try to
offer completion for topics as well.

<img src="https://storage.googleapis.com/wch/kafka-autocomplete.png" alt="kafka autocomplete screenshot" type="image/png" width="900">

---

The repository is provide under Apache 2.0 license. See LICENSE and NOTICE
for more information.
