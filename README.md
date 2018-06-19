# Kafka
ios oc＆swift ,Kafa<br>
第一步,设置kafka 地址<br>
KafkaClient.shareInstance().kafka(true, <br>withClient_Id: "aa",<br> withSocket_timeout: 1000, <br>withBroker: "60.26.117.22")<br>
第二步<br>
KafkaClient.shareInstance().sendMsg("aaa", <br>withTopic: "bbb", success: {<br>
            print("成功")<br>
        }) { (error) in<br>
            print("错误")<br>
            print(error)<br>
        }

