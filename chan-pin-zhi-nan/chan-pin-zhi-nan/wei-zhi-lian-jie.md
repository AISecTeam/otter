# 未知链接

恶意 URL 是网络钓鱼和传播恶意软件的最常见攻击媒介之一。攻击者通常会使用流行网站拼写错误的域，或者使用带有流行网站名称的子域，以试图诱骗用户信任链接。

这些 URL 在[间接提示注射](https://www.lakera.ai/blog/guide-to-prompt-injection#direct-prompt-injection-vs-indirect-prompt-injection)攻击者将某些内容嵌入到文档中，用作响应用户提示的上下文的攻击[检索增强生成](https://www.lakera.ai/blog/retrieval-augmented-generation)（RAG） 或类似的 GenAI 设置。

每当 LLM 从其他来源收到不受信任的内容以帮助响应最终用户时，都应该对其进行提示攻击筛查，并筛查 LLM 输出中的未知链接。这可以防止攻击者纵 LLM 显示网络钓鱼链接。



Unknown Links 检测器会标记不在前 100 万个 URL 中的 URL[最受欢迎的域名](https://www.domcop.com/top-10-million-domains).

可以通过添加已知的允许域列表来自定义它 应用程序，但可能不属于 Million Most Popular Domains 的一部分。这些值得信赖 在屏蔽内容中检测到域时，不会标记域。

可以通过策略添加允许的域。请参阅 [策略](https://docs.lakera.ai/docs/policies) 文档 以了解更多信息和执行此作的指南。



<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>



<figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>



