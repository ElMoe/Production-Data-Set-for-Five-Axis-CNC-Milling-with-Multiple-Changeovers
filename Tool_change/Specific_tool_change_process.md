# Specific conditions for tool change process of the underlying dataset:

## Loading of tools
1. The machine uses a chain magazine (Magazine, No. 1) with a buffer (Virtual magazine, No. 9998) and a loading station (Virtual magazine, No. 9999).
2. The tools on this machine can be loaded from the chain magazine into the spindle with a gripper device which has two places: 
- Spindle 1 = mag 9998, location 1
- Gripper 1 = mag 9998, location 2
- Gripper 2 = mag 9998, location 3
3. For general information on configuration see also Siemens documentation:
- https://support.industry.siemens.com/cs/mdm/109481649?c=43590384907&lc=de-DE
- https://support.industry.siemens.com/cs/mdm/109481649?c=43590384907&lc=en-DE
4. *Important remark for the underlying data set:*
- For the changeover process of the machine, the loading station on the backside of the machine was not used for the data set. All tools were loaded on the front opening the main machine door.
- The gripper device was used during production process of the machine.
- Please refer to the linked data set descriptor that explains the different phases of changeover and production.

## Gripper device
- The gripper device after the tool change is empty.
- See Gripper_in_action.mov for the tool change process with the gripper device.

## Chosen tool inventory management
1. As storing concept a chaotic inventory is used. A tool can have therefore different magazine places.
2. Only the 3D probe tool is always on place 4 of the magazine.

## Process of inserting new tools
1. Choose type of tool.
2. Choose tool name.
3. Parameters ST and D are set automatically by the machine.
4. Set length.
5. Set diameter.
6. Set number of teeth.
7. Set maximum rotational speed.
8. Set rotation direction.
9. Select coolant supply.

