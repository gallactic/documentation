Gallactic Keys
==============

`gallactic key` is a simple command-line tool working with gallactic keyfiles for account management. 

::
    $ gallactic key <command> [arguments...] [options...]

Manage accounts helps you to create new accounts, inspect existing account, sign a message/message file using ed25519 and change your password.

It supports interactive mode, when you are prompted for password as well as non-interactive mode where passwords are supplied via a given password file. Non-interactive mode is only meant for scripted use on test networks or known safe environments.

Make sure you remember the password you gave when creating a new account (with new, update or import). Without it you are not able to unlock your account.


create an account
^^^^^^^^^^^^^^^^^
Generates new keyfile. This keyfile is encrypted with the password you provide while creating a new account. You can specify the address type as 'ac' for accountAddress and 'va' for validatorAddress (By default account address [type: 'ac'] will be created)

:: 

    gallac

.. warning::
    Remember your password !