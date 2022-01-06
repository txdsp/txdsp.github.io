# Digital signal processing

Signals are [functions](https://en.wikipedia.org/wiki/Function_(mathematics)). They are catgorized based on if they are [sampled](sampling) and/or [quantized](quantization).

:::{panels}

**Continuous**
^^^
When a signal is defined for a range of [real numbers](https://en.wikipedia.org/wiki/Real_number), we refer to it as a "continuous signal."

---

**Discrete**
^^^
When a signal is [sampled](sampling), we refer to it as a "discrete signal," which is a type of [sequence](https://en.wikipedia.org/wiki/Sequence).

---

**Analog**
^^^
When the values of a signal are allowed to be an entire range of real numbers, we refer to it as an "analog signal." Depending on the context however, the term "analog" is often shorthand for "analog and continuous."

---

**Digital**
^^^
When a signal is [quantized](quantization) and can only take values from a [countable](https://en.wikipedia.org/wiki/Countable_set) set, we refer to it as a "digital signal." Depending on the context, the term "digital" is often shorthand for "digital and discrete."

:::

The "digital" in the phrase "digital signal processing" (DSP) is shorthand for "digital and discrete". Generically, a DSP system includes two devices:

:::{panels}

**[Analog-to-digital converter (ADC)](https://en.wikipedia.org/wiki/Analog-to-digital_converter)**
^^^
An ADC performs [sampling](sampling) and [quantization](quantization) on signals so that a computer processor can operate on them.

---

**[Digital-to-analog converter (DAC)](https://en.wikipedia.org/wiki/Digital-to-analog_converter)**
^^^
A DAC attempts to perform the opposite function of an ADC through [interpolation](https://en.wikipedia.org/wiki/Interpolation). Under [certain conditions](theorem-of-interpolation), the interpolation may be perfect.

:::


