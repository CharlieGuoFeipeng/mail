# mail
mail.properties
名称	类型	描述
mail.imap.user	串	IMAP的默认用户名。
mail.imap.host	串	要连接到的IMAP服务器。
mail.imap.port	int	要连接到的IMAP服务器端口，如果connect（）方法没有显式指定一个。 默认为143。
mail.imap.partialfetch	布尔	控制是否应使用IMAP部分抓取功能。 默认为true。
mail.imap.fetchsize	int	部分抓取大小（以字节为单位）。 默认为16K。
mail.imap.ignorebodystructuresize	布尔	IMAP BODYSTRUCTURE响应包括每个身体部位的确切大小。 通常，此大小用于确定为每个身体部位获取多少数据。 默认为false。
mail.imap.connectiontimeout	int	Socket连接超时值（以毫秒为单位）。 默认值为无限超时。
mail.imap.timeout	int	Socket I / O超时值（以毫秒为单位）。 默认值为无限超时。
mail.imap.statuscachetimeout	int	STATUS命令响应缓存的超时值（以毫秒为单位）。 默认值为1000（1秒）。 零禁用缓存。
mail.imap.appendbuffersize	int	追加到IMAP文件夹时，要在内存中缓冲的邮件的最大大小。
mail.imap.connectionpoolsize	int	连接池中的最大可用连接数。 默认值为1。
mail.imap.connectionpooltimeout	int	连接池连接的超时值（以毫秒为单位）。 默认值为45000（45秒）。
mail.imap.separatestoreconnection	布尔	用于指示是否对存储命令使用专用存储连接的标志。 默认值为false。
mail.imap.auth.login.disable	布尔	如果为true，则禁止使用非标准的AUTHENTICATE LOGIN命令，而是使用plain LOGIN命令。 默认值为false。
mail.imap.auth.plain.disable	布尔	如果为true，则阻止使用AUTHENTICATE PLAIN命令。 默认值为false。
mail.imap.auth.ntlm.disable	布尔	如果为true，则禁止使用AUTHENTICATE NTLM命令。 默认值为false。
mail.imap.proxyauth.user	串	如果服务器支持PROXYAUTH扩展，则此属性指定要充当的用户的名称。 使用管理员凭据对服务器进行身份验证。 身份验证后，IMAP提供程序将使用此属性中指定的用户名发出PROXYAUTH命令。
mail.imap.localaddress	串	创建IMAP套接字时要绑定到的本地地址（主机名）。 默认为Socket类选择的地址。
mail.imap.localport	int	创建IMAP套接字时要绑定到的本地端口号。 默认为Socket类选择的端口号。
mail.imap.sasl.enable	布尔	如果设置为true，则尝试使用javax.security.sasl程序包选择登录的认证机制。 默认为false。
mail.imap.sasl.mechanisms	串	要尝试使用的SASL机制名称的空格或逗号分隔列表。
mail.imap.sasl.authorizationid	串	在SASL认证中使用的授权ID。 如果未设置，则使用认证ID（用户名）。
mail.imap.sasl.realm	串	用于需要领域的SASL认证机制的领域，例如DIGEST-MD5。
mail.imap.auth.ntlm.domain	串	NTLM认证域。
mail.imap.auth.ntlm.flags	int	NTLM协议特定标志。
mail.imap.socketFactory	插座厂	如果设置为实现javax.net.SocketFactory接口的类，则此类将用于创建IMAP套接字。
mail.imap.socketFactory.class	串	如果设置，指定实现javax.net.SocketFactory接口的类的名称。 此类将用于创建IMAP套接字。
mail.imap.socketFactory.fallback	布尔	如果设置为true，则使用指定的套接字工厂类创建套接字失败将导致使用java.net.Socket类创建套接字。 默认为true。
mail.imap.socketFactory.port	int	指定在使用指定的套接字工厂时要连接到的端口。 未设置时使用默认端口。
mail.imap.ssl.enable	布尔	如果设置为true，则默认情况下使用SSL连接并使用SSL端口。 对于“imap”协议，默认为false，对于“imaps”协议为true。
mail.imap.ssl.checkserveridentity	布尔	如果设置为true，请检查RFC 2595指定的服务器标识。缺省值为false。
mail.imap.ssl.trust	串	如果设置，并且未指定套接字工厂，则启用使用MailSSLSocketFactory。 
如果设置为“*”，则所有主机都受信任。 
如果设置为以空格分隔的主机列表，则这些主机是受信任的。 
否则，信任取决于服务器提供的证书。
mail.imap.ssl.socketFactory	SSL插座厂	如果设置为扩展javax.net.ssl.SSLSocketFactory类的类，则此类将用于创建IMAP SSL套接字。
mail.imap.ssl.socketFactory.class	串	如果设置，指定扩展javax.net.ssl.SSLSocketFactory类的类的名称。 此类将用于创建IMAP SSL套接字。
mail.imap.ssl.socketFactory.port	int	指定在使用指定的套接字工厂时要连接到的端口。 如果未设置，将使用默认端口。
mail.imap.ssl.protocols	串	指定将为SSL连接启用的SSL协议。 属性值是javax.net.ssl.SSLSocket.setEnabledProtocols方法可接受的令牌的空格分隔列表。
mail.imap.starttls.enable	布尔	如果为true，则在发出任何登录命令之前，启用STARTTLS命令（如果服务器支持）将连接切换到受TLS保护的连接。 默认值为false。
mail.imap.starttls.required	布尔	如果为true，则需要使用STARTTLS命令。 如果服务器不支持STARTTLS命令，或命令失败，则connect方法将失败。 默认为false。
mail.imap.socks.host	串	指定将用于连接到邮件服务器的SOCKS5代理服务器的主机名。
mail.imap.socks.port	串	指定SOCKS5代理服务器的端口号。 只有在代理服务器未使用标准端口号1080时，才需要使用此选项。
mail.imap.minidletime	int	此属性设置以毫秒为单位的延迟。 如果未设置，则默认值为10毫秒。
mail.imap.enableimapevents	布尔	启用要传送到商店的ConnectionListener的特殊IMAP特定事件。 如果为true，则在Store的idle方法期间收到的未经请求的响应将作为ConnectionEvents发送，类型为IMAPStore.RESPONSE。 事件的邮件将是原始IMAP响应字符串。 默认情况下，不发送这些事件。
mail.imap.folder.class	串	com.sun.mail.imap.IMAPFolder的子类的类名。 子类可以用于提供对其他IMAP命令的支持。 子类必须具有公共构造函数public MyIMAPFolder（String fullName，char separator，IMAPStore store，Boolean isNamespace）和public MyIMAPFolder（ListInfo li，IMAPStore store）
