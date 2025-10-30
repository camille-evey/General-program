This python script is built to visualize the data recieved from the photodiode electronics via UDP. 

### class Box
The Box containing the widgets of use.
#### constructors
```python
class Box()
```
creates the Box object

#### methods
```python 
Box.processPendingDatagrams()
```
As long as the UDP has pending datagrams, read them and plots them via PlotData.

```python 
Box.PlotData(data)
```
decyphers the binary data recieved via UDP, and plots them on the graph.

```python
Box.Save()
```
Saves the processed data (WIP)


