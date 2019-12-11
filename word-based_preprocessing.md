# Word-based Audio Data Processing



## Reference

*   https://github.com/petewarden/extract_loudest_section



## Flow

-   Quality Check
    -   delete too small (e.g. ogg file size < 5kb)
    -   transform into 16kHz WAV files
    -   WAV with varying sample-rate is resmapled into 16KHz
-   Extract Loudest Section

    -   Overll volume: 16-bit sample data as the example, absoulte differences of the samples from zero (-32768 ~ 32767, -1.0 ~ 1.0), if volume is less than 0.4, delete it
-   Alignment

    -   Extracted the clip containing the highest overall volume
    -   Centralized the spoken word in the middle of trimmed clip
-   Manual Checking
    -   Check whether the audio is the same with word.
-   Background Noise
    -   Added several minute-long 16KHz WAV files of various kinds of background noise