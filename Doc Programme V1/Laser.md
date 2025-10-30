This python script is built to control the Koheron electronic card. 

### class CTL200
The instance of the electronic card
#### constructors
```python
class CTL200(port = 'COM7')
```
creates the object

#### methods
```python 
CTL200.send(txt)
```
sends an instruction to the card through the serial port. 

```python 
Box.close(dt)
```
Shuts down the card


### class Box
The Box containing the widgets of use.
#### constructors
```python
class Box(Laser = 'Laser1', port = 'COM7')
```
creates the Box object, with her title and the serial port used.

#### methods
```python 
Box.laser_onoff()
```
Depending on the button status, turns on or off the laser
```python 
Box.save_param()
```
Sends to the laser the two parameters.

```python
Box.update()
```
Reads the data of the two parameters and displays them into the interface

```python
Box.closeEvent(event)
```
Turns off the laser, and close the serial port.
