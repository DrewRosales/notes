Coding TODOList:
* Improve algorithms
* Work on C++ coding project
* Build devops containerization and workflow


Changing module parameters:

* ```which-machine [stack-module] [vehicle]```

* Change into machine in tmutt session

* `roscd` into module and change `default.yml`

* Relaunch `tmutt`



Recording MUTT data:
* Change to `record-data` in tmutt
* Add name of the rosbag
* End at the finish of each run

`argus_spaced.py` downsamples routes from existing argus routes

Remove Vahalla as global planner:
`grpc_bridge/config/default.yml` change the `use_mission_points_as_global_route` to `false`
