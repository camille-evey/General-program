This python script is built to pilots the photodiode electronics via UDP. 

### class Box
The Box containing the widgets of use.
#### constructors
```python
class Box()
```
creates the Box object

#### methods
```python 
Box.SendUDP(message)
```
Encodes and sends the message through the UDP port.

```python 
Box.SpinChanged(idx)
```
change the value of the spin of the "idx" parameter in order to know it has been changed

```python
Box.send_param()
```
When the "send" button is pressed, checks for each parameter if it has been changed (spin=1) or not (spin=0), and calls SendUDP for every parameters that have changed. 
