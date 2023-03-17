##############################################################
3. 隐私保护
##############################################################

标签：``隐私保护`` ``同态加密``  ``群/环签名``  ``WeDPR``

----

隐私保护是联盟链的一大技术挑战。为了保护链上数据、保障联盟成员隐私，并且保证监管的有效性，FISCO BCOS以[预编译合约](../../contract_develop/c++_contract/index.md)
的形式集成了同态加密、群/环签名验证功能，提供了多种隐私保护手段。此外，通过ZPK(零知识证明)以及WeDPR-Lab等一系列隐私保护项目保证链上链下数据隐私和信息安全。

**群/环签名：**
FISCOBCOS 支持一个群/环签名，群/环签名包括群签名(Group Signature)与环签名(Ring Signature)两个部分。

群签名是一种能保护签名者身份的具有相对匿名性的数字签名方案，用户可以代替自己所在的群对消息进行签名，而验证者可以验证该签名是否有效，但是并不知道签名属于哪一个群成员。同时，用户无法滥用这种匿名行为，因为群管理员可以通过群主私钥打开签名，暴露签名的归属信息。

环签名是一种特殊的群签名方案，但具备完全匿名性，即不存在管理员这个角色，所有成员可主动加入环，且签名无法被打开。

**同态加密：** 
同态加密本质是一种公钥加密算法，即加密使用公钥pk，解密使用私钥sk；并且支持密文计算。FISCO BCOS采用的是paillier加密算法，支持加法同态。paillier的公私钥兼容主流的RSA加密算法，接入门槛低。同时paillier作为一种轻量级的同态加密算法，计算开销小易被业务系统接受。

**ZPK：**
零知识证明


**WeDPR-Lab：**
WeDPR-Lab是一系列即时可用场景式隐私保护高效解决方案套件和服务。此方案致力于解决业务数字化中隐私不“隐”、共享协作不可控等隐私保护风险痛点，消除隐私主体的隐私顾虑和业务创新的合规壁垒，助力基于隐私数据的核心价值互联和新兴商业探索，营造公平、对等、共赢的多方数据协作环境，达成数据价值跨主体融合和数据治理的可控平衡。



.. toctree::
   :maxdepth: 1
 
   privacy.md
   zpk.md
   wedpr.md