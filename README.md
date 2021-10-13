# Republishing Linked Data Event Streams

This repository publishes or republished Linked Data Event Streams by using GitHub Actions.

## What data can be found in this repository?

At the moment you can find the following data:
- [A Linked Data Event Stream of the OSLO Knowledge Graph](https://ddvlanck.github.io/Republish-LDES/oslo-ldes-raw/1.trig) → GitHub does not resolve `.trig` extensions so it will automatically download. If you want to have a look at the data on GitHub, click [here](https://github.com/ddvlanck/Republish-LDES/tree/main/oslo-ldes-raw)
- [A substring fragmentation of the OSLO Knowledge Graph](https://ddvlanck.github.io/Republish-LDES/oslo-substring/root.ttl) → At this moment, the file extensions is `.ttl`, which is resolved by GitHub, but it should be changed to `.trig`.
- [A subject page fragmentation of municipalities in Flanders](https://ddvlanck.github.io/Republish-LDES/gemeente-subject-pages/11001.ttl) → There are no hypermedia controls yet, so to have a look at all subject pages, click [here](https://github.com/ddvlanck/Republish-LDES/tree/main/gemeente-subject-pages)
- [A substring fragmentation of municipality names in Flanders](https://ddvlanck.github.io/Republish-LDES/gemeente-substrings/root.ttl)

## Use

At the [TREE website](https://tree.linkeddatafragments.org/), there is an [autocompletion client](https://tree.linkeddatafragments.org/demo/autocompletion/) which lets you select a dataset of your own to experiment with. Enter one of the substring fragmentations as dataset and have fun!
- OSLO → https://ddvlanck.github.io/Republish-LDES/oslo-substring/root.ttl
- Municipalities in Flanders → https://ddvlanck.github.io/Republish-LDES/gemeente-substrings/root.ttl

## GitHub Actions

The publishing and republishing of Linked Data Event Streams in this repository are done by 2 independent GitHub Actions:
- [LDES Action](https://github.com/TREEcg/LDES-Action) → This action allows users to set a **fragmentation strategy** and then republish the original LDES with the chosen fragmentation strategy applied to it. In this repository, 2 fragmentation strategies were used: `substring`and `subject-pages`.
- [OSLO2LDES Action](https://github.com/ddvlanck/OSLO2LDES-Action) → This action publishes a Linked Data Event Stream of the OSLO Knowledge Graph, so no fragmentations yet.

