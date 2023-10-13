# Temporal Multiple Rotation Averaging: A Multi-Camera Dataset

For full details on the motivation, setup and use of this dataset, consult the following paper:
Aidan Blair, Amirali K. Gostar, Edmundo Guerra Paradas, Antoni Grau, Alireza Bab-Hadiashar and Reza Hoseinnezhad, "Temporal Multiple Rotation Averaging: A Multi-Camera Dataset", ICCAIS 2023.

## Usage

The dataset comprises three parts:
* The ground truth camera poses (translations and orientations). Data is stored in individual xlsx files for each camera and each scenario. Eaach row is the ground truth value for a single timestep, in descending order, with the top row containing the labels 'Xpos', 'Ypos', 'Zpos', 'X', 'Y', 'Z', 'W' for the columns. The first three columns are the camera translations in Cartesian coordinates, the last four clumns are the camera orientations in quaternions.
* The images. The images are storeed in individual directories for each scenario. The images are labelled in the form 'camX_Y_Z.jpg', where 'X' is the camera id, 'Y' is the scenario time step, and 'Z' is the Unix timestamp.
* The metadata. This includes a file for each camera containing the camera paremeters, labelled 'camXparams.txt'

## License

[CC-BY-4.0](https://choosealicense.com/licenses/cc-by-4.0/)