In the files, each line represents the semantic annotations for an image and follows the format below:

`ID PLACECTG OBJ1 OBJ2 OBJ3 OBJ4 OBJ5 OBJ6 OBJ7 OBJ8 OBJ9 OBJ10`

- `ID` = identification number of the image in the data sequence;
- `PLACECTG` =  the place category of the image. The values are in numeric format and vary as follows: 0 (bathroom), 1 (bedroom), 2 (corridor), 3 (home office), 4 (kitchen), and  5 (living room);
- `OBJi` = `i` is the identifier of an object category and varies as follows: 1 (chair), 2 (couch), 3 (bed), 4 (dining table), 5 (toilet), 6 (TV), 7 (laptop), 8 (oven), 9 (sink), and 10 (refrigerator). The value of each `OBJi` field is 1, for the presence of the object category in the room, or 0, for its absence.
