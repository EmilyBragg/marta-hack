Project:
    mapping all locations that are accessible by public transit and up to N minutes of walking

Parameters:
    starting point
    number of connections
    total time
    total walking time (split?)

steps:
1) find the nearest transit stations on each line
2) find all stops within the total time (not looking at timetables)
3) find the isolines for each stop (filtering out duplicates) in min(max walking time - walk to station, total_time - walk_to_station - time_on_train)
4) plot all isolines on the same map

(Potential improvement - overlay that with a map of how far you could go on a car in the same time)
