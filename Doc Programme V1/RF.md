This python script is built to pilots the RF synthetiser.
### class Worker
The worker is used to launch a parallel action in a program. Here, we use it to check constantly if the RF is locked or not.
#### constructors
```python
class Worker()
```
Creates a worker for the lock status
#### Slots
```python
Worker.run()
```
sends an order to recieve the lock status each 0.5sec.


### class Box
The main window of the programm.
#### constructors

```python
class Box(path)
```
creates the Box object
#### methods

```python
Box.FreqTune()
```
Sends a new frequency to the RF.

```python 
Box.PowTune()
```
Sends a new power to the RF

```python 
Box.IsLocked()
```
Checks the results of the worker.run methods, and changes the LED according to the lock status.


