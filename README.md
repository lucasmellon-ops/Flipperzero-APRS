# FlipperZero-APRS Project

## Introduction

The FlipperZero-APRS project aims to explore the capabilities of Flipper Zero in receiving and decoding APRS (Automatic Packet Reporting System) packets. Flipper Zero's hardware, including its CC1101 sub-GHz module, has presented both opportunities and challenges in implementing APRS. This README aims to outline the project's goals and address some of the hardware problems faced along with solutions.

## Outline

### Capabilities

- **Reception of APRS Packets**: The main goal is to enable Flipper Zero to receive APRS packets.
- **Exploration of CC1101**: Utilizing the existing [RadioLib](https://github.com/jgromes/RadioLib) library to interact with Flipper Zero's CC1101.
- **Frequency Restrictions**: Finding ways to bypass the restrictions in place to meet part 15 for the device.

### Hardware Challenges

1. **Transmission Range**: The limited transmission range of the Flipper's CC1101 poses a significant obstacle.
2. **Lack of GPS**: Although GPS is not required for receive or transmit, it might be necessary for specific applications.
3. **Lack of a TNC (Terminal Node Controller)**: Hardware for modem functions and audio in/out to properly rx/tx APRS packets would need to be added.

### Solutions

- **Software-Based TNC**: TCN can be done in software. This option, while potentially limited, should be explored.
- **Exploration of Different Frequencies**: APRS can be used on any radio frequency. There are existing sub-GHz projects that use APRS on LoRa, for example.
- **Potential PCB Implementation**: A customized PCB build like Mobilinkd TNC might be necessary to handle the TNC functionalities.

## Collaboration

The project is in its early stages, and collaboration is welcome! Discussions on how best to move forward with this project are ongoing on Discord. Join in if you'd like to contribute.

## References

- [RadioLib for APRS Implementation](https://github.com/jgromes/RadioLib)
- [Flipper Zero Official Page](https://flipperzero.one/)

## Disclaimer

This project is experimental and under active development. Some theories and implementation details might change as the project progresses. Use this information and code at your own risk.

## Acknowledgments

Thanks to the community, especially contributors like Zve8, federalfarmer_xyz, BrotherCagliostro, and others who have provided valuable insights and comments on this exploration.
