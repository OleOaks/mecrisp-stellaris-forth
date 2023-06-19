Tera Term
=========

What's this used for?
---------------------

The normal way of communcating with Forth is through a VT100 serial terminal emulator, one example being the free open-source Tera Term.

Forth provides a command line through USART which is typically connected through an inexpensive USART to USB serial converter like a :doc:`/workbench/hardware/cp2102` board. The CP2102 plugs into a usb port on the computer with which Term Term communicates.

Where to get it?
----------------

Tera Term is freely downloaded from `Tera Term homepage`_.

.. _Tera Term homepage: https://ttssh2.osdn.jp/index.html.en


Setup Tera Term Quicksteps
--------------------------

#. Plug the :doc:`/workbench/hardware/cp2102` board into computer.
#. Open the Tera Term application. (It defaults to a TCP/IP connection)
#. Select the 'Serial' connection option, and click 'OK'. (a COM port should be displayed in the 'Port:' textbox).
#. Goto 'Setup' --> 'Serial' dialog.
#. Change 'Speed' to 115200, or whatever your Forth installation will default to. Then click 'New setting' to dismiss the dialog box.
#. Hit the 'Enter' key on your keyboard. You should see an 'ok.' response from Forth!
#. Goto 'Setup' --> 'Terminal' dialog.
#. Change the New-line Receive value from 'CR' to 'LF', then click 'OK' to dismiss the dialog box.
#. Goto 'Setup' --> 'Font' -- 'Font' dialog.
#. I change the font to 'Courier New' and the size to '12', then click 'OK' to dismiss the dialog box.
#. The default Tera Term window size is a bit small, stretch it to a comfortable size.
#. Goto 'Setup' --> 'Save setup...' and create a filename to remember these settings.
#. The next time you open Tera Term, goto 'Setup' --> 'Restore setup...' and find your saved settings.

Press the reset button on the microcrontroller, a startup message should be displayed in Tera Term...

``Mecrips-Stellaris 2.6.5 for STM32F103 by Matthias Koch``

Tera Term setup screenshots
---------------------------

.. figure:: teraterm_open.png

   *Defaults to a TCP/IP connection when first opened*

.. figure:: teraterm_selectserial.png

   *Select the 'Serial' connection option, then click 'OK'*

.. figure:: teraterm_serialdialog.png

   *Goto 'Setup' --> 'Serial port...' dialog box*

.. figure:: teraterm_baud.png

   *Change 'Speed' to 115200, or whatever your Forth installation requires*

.. figure:: teraterm_ok.png

   *Press the 'Enter' key on your keyboard. You should see an 'ok.' response from Forth!*

.. figure:: teraterm_terminaldialog.png

   *Goto 'Setup' --> 'Terminal' dialog box*

.. figure:: teraterm_lf.png

   *Change the New-line Receive value from 'CR to 'LF', then click 'OK' to dismiss the dialog box*

.. figure:: teraterm_fontdialog.png

   *Goto 'Setup' --> 'Font' -- 'Font' dialog box*

.. figure:: teraterm_font.png

   *Optionally -- Change the font to 'Courier New' and the size to '12', then click 'OK' to dismiss the dialog box*

11. Resize the Tera Term window if it's too small for normal use

.. figure:: teraterm_savedialog.png

   *Goto 'Setup' --> 'Save setup..' and create a filename to remember these settings*

.. figure:: teraterm_restoredialog.png

   *The next time you open Tera Term, goto 'Setup' --> 'Restore setup...' and find your saved settings*



