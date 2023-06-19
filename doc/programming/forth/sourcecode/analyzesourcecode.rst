Source Code
===========

The following is my attempt at understanding how the source code is assembled into machine code. I'm using a STM32F103 BluePill as an example.

Instructions starting with a :code:`.` are assembler directives. Here is a link to `ARM-Directives`_

.. _ARM-Directives: https://sourceware.org/binutils/docs/as/ARM-Directives.html

.. code-block::

    .syntax unified


This line establishes the `Instruction Set Syntax`_. Essentially :code:`unified` is the newer syntax for ARM.

.. _Instruction Set Syntax: https://sourceware.org/binutils/docs/as/ARM_002dInstruction_002dSet.html

.. code-block::

    .cpu cortex-m3



