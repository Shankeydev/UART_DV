# UART_DV
This is a project for design and verification of UART (Universal Asynchronous Receiver-Transmitter) protocol.
the design part contains 1) clock generator which generates the clock for transmitter and reciever based on given baud rate.
here i have taken the reciever clock to be 16 times fater than transmittor clock and the data in reciever is being sampled at each 8th pulse of the reciever clock.
For checking error in transmitted and recieved data parity bit checker is used, and user has to choose either he needs parity bit or not, if yes which type of parity (odd /even).
User has to specify the length of data (rangng from 5 to 8 bits).
Transmitter, Reciever and clock generator are then instantiated in top module to make a connection between them.
Verification environment is written in UVM and it contain all the possible sequences to drive the DUT.
