# semantic_annotations_sun3d

Semantic annotations of the RGB images from 5 paths of the [SUN3D](https://sun3d.cs.princeton.edu/) dataset, one data sequence from each selected path. More details below:
- The paths are `home_at`, `home_han`, `home_md`, `home_puigpunyen`, and `home_rz`;
- The RGB images of the selected data sequence from each path were annotated with 6 place categories and 10 object categories;
- From the home_md path, the data sequence 9 (out of 10 available) was the one selected. From home_puigpunyen, the data sequence 2 (out of 4 available) was the one selected. The other selected paths have only one data sequence available;
- The RGB images received the most appropriate place category (out of the 6) and all objects present in the room (out of the 10 selected) as ground truth, i.e., each image received as ground truth a 10-dimensional vector with the presence of all objects in the room, not those visualized in the image;
- The place categories were `bathroom`, `bedroom`, `corridor`, `home office`, `kitchen`, and `living room`;
- The object categories were `chair`, `couch`, `bed`, `dining table`, `toilet`, `TV`, `laptop`, `oven`, `sink`, and `refrigerator`.

The semantic annotations were made in a real-time process and therefore the loss of some image frames during the annotation processes was expected. However, fortunately, a very small number of RGB frames was lost in most paths (6 in home_at, 2 in home_md, 1 in home_puigpunyen, and 42 in home_rz) and only in path home_han a larger number (558) was lost, which represents approximately 6.5% of the total number.

## Files

The semantic annotations can be found in the `files` folder, where there is a file for each path containing the following data for each annotated image: id of the image; place category (in numeric format); and 10-dimensional objects vector.

Originally, a file was generated for each path also containing a spatial position vector and a visual features vector for each image (obtained using ORBSLAM2 and MobileNetV2, respectively). However, the files available in this repository only contain the essential information, that is, the ids of the images and the semantic labels. The original files, with the complete information, will be made available in a different location soon.

## More information

The semantic annotations were made as part of my PhD research. You can find more information about them and the annotation process in my PhD thesis (Chapter 5, Sections 5.4.2.1 to 5.4.2.5)), available [here](https://repositorio.ufpe.br/handle/123456789/55203).

## Citation 

If you use the semantic annotations, please cite my thesis as below.

- SOUSA, Ygor César Nogueira. A new approach to semantic mapping using reusable consolidated visual representations. Thesis (PhD in Computer Science) – Universidade Federal de Pernambuco, Recife, 2023.
