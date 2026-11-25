# adaptive-driver-warning-system

# Adaptive Driver Warning System

## Project Overview

The prototype explores the impact of false collision warnings
on driver responsiveness and demonstrates how an adaptive
warning system can modify its detection threshold in response
to detection errors.


## Project Status

Functional browser-based simulation prototype.

Implemented features:

- Interactive driving scenarios
- Simulated sensor uncertainty
- Collision risk estimation
- Threshold-based warning decisions
- Adjustable warning sensitivity
- Rule-based adaptive warning algorithm
- Driver response controls
- Response time measurement
- Detection performance statistics
- Individual trial history
- Simulation reset controls
- Responsive user interface

## Technologies Used

- HTML5: Interface structure
- CSS3: Visual design and responsive layout
- JavaScript: Simulation logic, adaptive algorithm,
  interaction handling and performance tracking
- GitHub: Version control and project documentation

## Running the Prototype

1. Download index.html from this repository.
2. Open the file in a modern web browser.
3. Select a warning sensitivity mode.
4. Select a driving scenario.
5. Respond to collision warnings using the available controls.
6. Review performance statistics and trial history.
7. Reset the simulation to begin another session.

No external libraries, installations or server are required.

## Intelligent System

The system uses a rule-based adaptive detection algorithm.

Simulated sensor uncertainty is added to a predefined
scenario risk score. The resulting score is compared
against a warning threshold.

In adaptive mode:

- False alarms increase the threshold by 5 percentage points.
- Missed hazards decrease the threshold by 10 percentage points.
- Correct detection outcomes maintain the existing threshold.

The adaptive threshold is restricted to values between
30 and 80 percent.

The algorithm prioritises avoiding missed hazards by
applying a larger adjustment following a miss.

## Development Record

The prototype was developed incrementally using GitHub
version control.

| Stage | Development change | Rationale |
|---|---|---|
| 1 | Initial HTML interface | Establish the simulator structure |
| 2 | Dashboard styling | Improve visual readability |
| 3 | Scenario selection | Enable interactive simulation |
| 4 | Risk estimation | Represent different hazard severities |
| 5 | Warning decisions | Implement a detection criterion |
| 6 | Sensor uncertainty | Simulate false alarms and missed hazards |
| 7 | Adjustable sensitivity | Explore detection trade-offs |
| 8 | Driver response controls | Measure user responsiveness |
| 9 | Performance statistics | Support quantitative evaluation |
| 10 | Adaptive algorithm | Automatically modify warning sensitivity |
| 11 | Trial history and reset | Support repeatable evaluation sessions |
| 12 | Interface improvements | Improve visual hierarchy and usability |
| 13 | Documentation | Explain implementation and operation |

## AI Assistance

AI was used during development to assist with:

- Structuring the incremental development process.
- Designing the rule-based adaptive algorithm.
- Identifying and correcting duplicated JavaScript.
- Suggesting functional test cases.

## Limitations

- Driving scenarios and sensor readings are simulated.
- Risk scores are not calibrated collision probabilities.
- The adaptive algorithm relies on simulated ground truth.
- Threshold values are illustrative design parameters.
- Response times represent browser interactions rather
  than real driving behaviour.
- Driver trust is not directly measured.
- Results are stored temporarily and lost on refresh.
- The prototype is not intended for real vehicle deployment.

## Future Improvements

- More realistic driving environments.
- Integration with real or recorded sensor data.
- Audio and multimodal collision warnings.
- Direct measurement of driver trust.
- Controlled participant evaluation.
- Persistent storage and export of experimental results.

## Repository Files

- index.html: Complete interactive simulation.
- README.md: Project documentation.



## Functional Testing

| Test | Result |
|---|---|
| HTML opens without errors | Pass |
| All three driving scenarios work | Pass |
| Risk scores vary between trials | Pass |
| Warning decisions follow the threshold | Pass |
| All four sensitivity modes work | Pass |
| False alarms and misses are recorded | Pass |
| Threshold increases after false alarms | Pass |
| Threshold decreases after missed hazards | Pass |
| Brake and ignore controls work | Pass |
| Reaction times are recorded | Pass |
| Performance statistics calculate correctly | Pass |
| Trial history records each scenario | Pass |
| Reset clears statistics and history | Pass |
| Interface displays correctly | Pass |

All 14 functional tests passed.


