# Kafka
ios oc＆swift ,Kafa
第一步,设置kafka 地址
KafkaClient.shareInstance().kafka(true, withClient_Id: "aa", withSocket_timeout: 1000, withBroker: "60.26.117.22")
第二步
KafkaClient.shareInstance().sendMsg("aaa", withTopic: "bbb", success: {
            print("成功")
        }) { (error) in
            print("错误")
            print(error)
        }
