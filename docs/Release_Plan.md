# Release Plan

## Size Estimates (LOC)

Each column specifies estimated and actual values at the beginning of that iteration. For example, at the beginning of iteration 2 you know the actual size of the code integrated during iteration 1 and based on your experience during iteration 1 you can update the estimated size values for the subsequent iterations.

**Client**

| Client | Login | Registration | Start apllication | |
| --- |:---:|:---:|:---:|:---:|
| Login | 50 | 70 |  |
| Registration | 100 | 100 | 310 |
| Message | 200 | 200 | 200 | 600 |
| **Total:** | 350 | 370 | 510 | 600 |

**Server**

| Server | Grant multiconnectons | Login | Private message ||
| --- |:---:|:---:|:---:|:---:|
| Grant multiconnectons | 15 | 20 |
| Login | 25 | 25 | 58 |
| Private message | 25 | 25 | 25 | 84 |
| **Total:** | 65 | 70 | 83 | 84 |



## Effort Estimates (Minutes)

**Client**

| Client | Login | Registration | Start apllication | |
| --- |:---:|:---:|:---:|:---:|
| Login | 30m | 1h |   |
| Registration | 45m | 45m | 2h |
| Message | 1h | 1h | 1h | 2h 30m|
| **Total:** | 2h 15m | 2h 45m | 3h | 2h 30m|

**Server**

| Server | Grant multiconnectons | Login | Private message | |
| --- |:---:|:---:|:---:|:---:|
| Grant multiconnectons | 20m | 45m |   |
| Login | 1h | 1h | 2h |
| Private message | 1h 45m | 1h 45m | 1h 45m | 3h 30m |
| **Total:** | 3h 05m | 3h 30m | 3h 45m | 3h 30m |

## **Client**

### Login
| Feature | Estimated Effort | Actual Effort |
| --- |:---:|:---:|
| Account control | 10m | 20m |
| Graphic login | 20m | 40m |
| **Total:** | 30m | 1h |

### Registration
| Feature | Estimated Effort | Actual Effort |
| --- |:---:|:---:|
| Registration | 20 m | 30m|
| Graphic registration | 20 m | 30m|
| **Total:** | 40m | 1h |

### Message
| Feature | Estimated Effort | Actual Effort |
| --- |:---:|:---:|
| Private mesage | 20m | 30m |
| Graphic message | 30m | 1h |
| **Total:** | 50m | 1h 30m |

## **Server**

### Grant multiconnectons
| Feature | Estimated Effort | Actual Effort |
| --- |:---:|:---:|
| Create array users | 05m | 05m |
| Enable multi-threading | 10m | 25m |
| Add the user to the user array | 15m | 15m |
| **Total:** | 20m | 45m |

### Login
| Feature | Estimated Effort | Actual Effort |
| --- |:---:|:---:|
| Reciving the request from the client | 15m | 25m |
| Converting into string the byte | 15m | 1h |
| Reading from the file | 30m | 35m |
| **Total:** | 1h | 2h |

### Private message
| Feature | Estimated Effort | Actual Effort |
| --- |:---:|:---:|
| Enter in the function privateMessage | 20m | 1h |
| Create the packet to send | 50m | 1h 15m |
| Send the packet  | 35m | 1h 15m |
| **Total:** | 1h 45m | 3h 30m |




## **Features we would like to add in the future**

**Client**

| Feature | Effort Estimate |
| --- |:---:|
| Possibility to create group chat, for example if i want to send a message directly to my friends | 2-3 hrs |
| Possibility to customize the client chat apllication (background, font and other things) | 4-5 hrs |
| Possibility to customize your profle and the possibility to see the other user profile | 3-4 hrs |

**Server**

| Feature | Effort Estimate |
| --- |:---:|
| Add the user list request | 1h |
| Add more security control | 1h 45m |
| Put the user information inside a database | 2h |
