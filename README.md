# ccTest<br />
**Created Date:** 12/2/2009<br />
**Last Updated:** 10/12/2010<br />
**Description:** A UI Toolkit program that maintains a simple credit card file, and uses the new data encryption routines in 9.3, with a utility class that has routines to validate credit card numbers and another class that can expose the data encryption with non-synergy data types. (Update for Synergy 9.5 compatibility)<br />
**Platforms:** Windows; Unix; OpenVMS<br />
**Products:** Synergy DBL; UI Toolkit<br />
**Minimum Version:** 9.3.1<br />
**Author:** William Hawkins
<hr>

**Additional Information:**
The source files enclosed in this zip files are:

ccTest.dbl
This is a Synergy/DE UI Toolkit test program that manages a simple Synergy DBMS isam file.
This file contains basic credit card information, as defined in the file ccrec.inc.
Based upon the defines near the top of the file, various encryption options can be
exercised by this program. The defines can change the format of the data file, as some
encryption options require additional record space to save the encrypted data.

CCutils.dbc
This file contains a few utility methods used in the validation of credit card numbers.

Encryption.dbc
This file contains a data encryption class, that can be used to encrypt data.
You will need to adjust the logic in the method getEncryptionCode() so that the
encryption code is correctly managed. Currently this uses the Synergy License Manager
licensee name as the encryption code.

Build.bat
Windows/Unix build command file
