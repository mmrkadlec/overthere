# Project "overthere"
Runs something on a remote machine, ie. over there.

# TODO
* determine semantics of delete, mkdir, mkdirs, renameTo with respect to errors.
* factor out dependencies that might cause a version clash for users of this library such as google collections and apache commons.
* port scp -r functionality.
* figure out what to do with the HostFileInputStreamTransformer filter.
* figure out what to do with HostFileUtils.
  * move copy to OverthereFile?
* decide whether to support winsshd and/or copssh and/or other Windows SSH implementations. Leave that up to subclasses?
* implement SSH pub/private key implementation in a nicer manner.
* implement not-removing temporary directories in a nicer manner, or at least with a more up-to-date key name.
* remove HostConnection.copyToTemporaryFile?
* redesign InputResponse map?
* rename HostConnection to OverthereConnection?
* reimplement tunneled SSH connections.
* add OverthereFile.valueOf().
* add WrappingOverthereFile to tunnel to other java.io.File implementations.
* need to be able to set default values for synehtic properties (port).
* need to be able to define abstract synthetic types (SshHost). Then temporaryDirectoryPath could also be defined in an abstract base class below Host.
