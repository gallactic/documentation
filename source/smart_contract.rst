Smart contracts in Gallactic
============================

.. _simple-smart-contract:

***********
hello world
***********

Let us begin with the most basic example. It is fine if you do not understand everything
right now, it is just to run a simple contract in gallactic network.

::

    pragma solidity ^0.4.25;

    contract SimpleStorage {
        uint storedData;

        function set(uint x) public {
            storedData = x;
        }

        function get() public view returns (uint) {
            return storedData;
        }
    }