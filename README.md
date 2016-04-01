# Pynq
(Py)thon on Zy(nq)


## Zybo image files

- All images including the latest are available here: 
```
file://xsj-pvstd2t01-w/xrlabs/grahams/public/ubuntu-core-zybo/
```

- After imaging, change Zybo's hostname to avoid network conflicts
```
sudo sh -c 'echo "UNIQUE_NAME" > /etc/hostname'
sudo shutdown -r now
```


## Updating `pynq` on Zybo using pip 

```
sudo -H pip install -e 'git+https://github.com/Xilinx/Pynq@master#egg=pynq&subdirectory=python'
```

## Running Regression from terminal
```
py.test –vsrw
```