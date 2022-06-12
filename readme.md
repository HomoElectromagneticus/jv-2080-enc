This PCBA design implements a replacement for the main "value" encoder on the Roland JV-2080 synthesizer. This is useful because the original part is no longer manufactured.

In short, this design leverages work available on mitxela.com, namely: https://mitxela.com/projects/jv1080_encoder_repair. The code shown on that page creates an elegant low-power interface between a standard rotary encoder commonly available at the time of this writing and what the JV-2080 expects. I encourage any reader here to explore that page to learn more.

You may find the necessary files to build this project for yourself on the "Releases" section of this repository page. Note that you will also need the pre-compiled binary to flash onto the ATTiny13A as well as a means to flash it. You may find the pre-compiled binary here: https://github.com/mitxela/jv1080-encoder. Pay attention to the fuse settings required for the microcontroller: 
  - high fuse byte -> 0xFF 
  - low fuse -> 0x73

These will need to be set when flashing the ATTiny13A.

For more information about the process, please visit https://homoelectromagneticus.com/projects/jv_2080_enc.php. If you try this project for yourself and run into a problem, do not hesitate to create an issue in this repository and I will do my best to help you.
