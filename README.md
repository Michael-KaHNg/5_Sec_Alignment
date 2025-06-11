


# 5_Sec_Alignment (Adjust Arduino Timestamp to GPIO) [P6_3]
# use CAIMAN environmnet

# Need
1. Arudino behavioral text file (.txt)
2. HDF5 file (.hdf5)
3. GPIO file (.csv, Export with "First data iterm's time" **  )
##################################################################################################
# Check Alignmnet Results

1. Make Sure the data length is the same for [Length of cell] AND [GPIO_Corrected_FramesImaged]  (eg 48001) (in a 40 minute session @ 20 frames per second)
2. [Actual number of 5s pulse] should be 480 (in a 40 minute imaging session)
3. The numbers of Start/End, ON/OFF, IN/OUT timestamps should match up

![Fig_1](https://github.com/user-attachments/assets/e441cc5e-1c54-4139-bc69-976f21b23e41)

##################################################################################################
# Check that you have the right files.  The IR data (bottom) should match up between GPIO and Arduino
![Fig_2](https://github.com/user-attachments/assets/c94090c5-7026-43c2-9bd4-4766f717d705)

##################################################################################################
# The 5s pulse duration should be very close to 5s (Top) 
# and within the red lines (bottom) 

If there are points outside the two red lines (> 10,000 ms or < 2,500 ms ), the pulses are not detecting correctly.   
You will need to check the 5s pulse graph to adjust the threshold for 5 second pluse detections. 

![Fig_3](https://github.com/user-attachments/assets/89543b06-55d4-4bbc-86fc-0aef0fe8c96e)

![Fig_5](https://github.com/user-attachments/assets/a4c0e486-538f-429d-942b-c880c0a5ffba)
![Fig_6](https://github.com/user-attachments/assets/495f7c8f-fb55-40f2-91a9-c968b173f7b5)
![Fig_7](https://github.com/user-attachments/assets/4ee8d177-c37e-4777-8358-86e1c22d1646)
![Fig_8](https://github.com/user-attachments/assets/6e3ca1a7-2cf7-47c9-85f6-04ed1848a367)
