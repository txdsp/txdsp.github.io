# Digital Communications

Digital communication occurs in a wide range of contexts. Depending on the constraints and requirements, the bitrate of common digital communication protocols may vary in [data rate](https://en.wikipedia.org/wiki/Bit_rate) from a few kbit/s up to 100s of Tbit/s.

:::{panels}

**[Wireline](https://en.wikipedia.org/wiki/Wired_communication)**
^^^
When the transmitter and receiver are stationary, we can simply connect them with conducting, fiber-optic, or other specially designed transmission wires. Wireline communication systems typically have low noise, minimal interference and can achieve high data rates.

* USB cable between PC and peripheral<br>(100s or 1000s of Mbits/s)
* PCI link between CPU and GPU<br>(100s or 1000s of Gbits/s)
* 5000km fiber-optic internet connection<br>(10s or 100s of Tbits/s)

---

**[Wireless](https://en.wikipedia.org/wiki/Wireless)**
^^^
When the transmitter and/or receiver can't be connected by a transmission line, we can use acoustic, radio, light, or other types of [waves](https://en.wikipedia.org/wiki/Wave) to perform digital communication. Typically, these modes are much more susceptible to noise and interference.
* Underwater acoustic modem<br>(100s or 1000s of bits/s)
* Digital radio station<br>(~100 kbit/s)
* Bluetooth/WiFi/Cellular<br>(100s or 1000s of Mbits/s)

---

**[Synchronous](https://en.wikipedia.org/wiki/Synchronous_serial_communication)**
^^^
A clock signal is shared between the transmitter and receiver which greatly simplifies the digital communication process.

* SPI connection between microcontroller and ADC/DAC

---

**[Asynchronous](https://en.wikipedia.org/wiki/Asynchronous_serial_communication)**
^^^
When there is no shared clock signal, the data stream is structured to allow inference of the clock signal.

* Communication between microcontroller's UART and MIDI device

---

**[Baseband / Line code](https://en.wikipedia.org/wiki/Line_code)**
^^^
If the transmission medium supports all frequencies from zero hertz up to some maximum bandwidth B, and if only one pair of users or devices has access to the medium, then we are free to use any and all frequencies (up to B) for the digital communication.

---

**[Modulated / Frequency-division](https://en.wikipedia.org/wiki/Frequency-division_multiplexing)**
^^^
If the transmission medium only supports a narrow band of frequencies or is shared by several users or devices, it is common to allocate frequency sub-bands to specific users. This is achieved by modulation, the process of shifting a signal to a specific frequency band.

:::

An example of digital communication that is wireline, synchronous, and baseband is the transmission of uncompressed video from a PC to a monitor via HDMI. These types of systems typically require little or no use of digital signal processing.

In contrast, a communications satellite performs wireless, asynchronous, and frequency modulated communications. Systems with these characteristics often require several subsystems to perform tasks such as modulation, filtering, equalization, coding, and encryption. Though it's possible to perform these with dedicated hardware, it is often advantageous to implement one or more of these subsystems in software In this case we refer to the system as a software defined radio (SDR). DSP theory and algorithms form a foundation on which to design and implement SDRs.