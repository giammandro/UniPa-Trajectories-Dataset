*************************************
****** pois.csv Data Structure ******
*************************************

* ID: unique integer id for every Point of Interest (PoI);
* semantic_flag: brief description of the PoIs semantic labels which capture intended functionality of that region;
* latitude: latitude coordinate for the PoI;
* longitude: longitude coordinate for the PoI;
* description: caption for the PoI (in Italian);
* semantic_flag_description: caption of the PoI semantic class.

*************************************
** trajectories.csv Data Structure **
*************************************

* uid: unique integer id for every user;
* user_behavioral_profile: id of the user behavioral profile which captures the different mobility behavioral patterns;
* date: date of the trajectory in format YYYY-MM-DD;
* arrival_times: we split the day in 48 time slots (ranging from 0 to 47), then, arrival_times is a list of integers which represents the arrival time slot in the corresponding PoI of the trajectory;
* permanence_times: is a list of integers which represents the amount of minutes the user stayed in the corresponding PoI of the trajectory;
* trajectory: is a list of the visited PoIs IDs;
* sem_trajectory: is a list of the visited PoIs semantic flags.