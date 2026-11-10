# getorganelledb — GetOrganelle default databases 0.0.1

A mirror of `v0.0.1.tar.gz` from [Kinggerm/GetOrganelleDB](https://github.com/Kinggerm/GetOrganelleDB/releases/tag/0.0.1)
(the seed and label databases of every organelle type: animal_mt, fungus_mt, fungus_nr, embplant_pt,
embplant_mt, embplant_nr, other_pt), byte for byte as `getorganelledb-0.0.1.tar.gz` (md5 `3cb019f4fda673fedceba2fa33ac4b24`).
MitOmics installs it with GetOrganelle's own offline route instead of downloading it in every task:

    wget https://raw.githubusercontent.com/zampini28/getorganelledb/refs/heads/main/getorganelledb-0.0.1.tar.gz
    echo "3cb019f4fda673fedceba2fa33ac4b24  getorganelledb-0.0.1.tar.gz" | md5sum -c -
    tar xzf getorganelledb-0.0.1.tar.gz         # -> 0.0.1/{SeedDatabase,LabelDatabase}
    get_organelle_config.py -a animal_mt --use-local 0.0.1 --config-dir godb

**Authors:** Jian-Jun Jin and the GetOrganelle contributors. Jin J-J, Yu W-B, Yang J-B, Song Y, dePamphilis CW,
Yi T-S, Li D-Z (2020) GetOrganelle: a fast and versatile toolkit for accurate de novo assembly of organelle
genomes. *Genome Biology* 21:241.

**License:** GNU General Public License v3.0, as upstream (copy in `LICENSE`). Unmodified.
