# 微信会员、商城会员、连锁会员与会员中心数据交互接口(vip)

1. 读取会员信息
````php
    /* @desc [获取会员的消息]
     * @param $vid intger  [会员id]
     * @param $fields string  [提取字段，默认所有]
     * @return $array []
     * @return $data['status']   1成功  0失败
     * @return $data['data']   会员信息  name姓名 account账户余额  point积分
    */
    SnsApi::cApi('Vip/get',array('vid'=>会员的vid,'fields'=>"*"));
````


2. 读取会员信息
````php
    /* @desc [添加会员]
     * @param $info  array  [会员基础信息]
     * @param $name[会员姓名], $phone[会员手机号或座机号], $type[微信1、商城2、连锁3] 
     * @return $array []
     * @return $data['vid']   会员vid
     * @return $data['status']   1成功  0失败
    */
    SnsApi::cApi('Vip/add',$info);
````



3. 更新会员信息（余额更改，积分更改，手机号更改）
````php
   
    /* @desc [更新会员]
     * @param $info  array  [会员基础信息]
     * @param $name[会员姓名], $phone[会员手机号或座机号], $account[会员余额，充值为正数，消费为负数],$point[会员积分，增加为正数，扣除为负数]
     * @return $array []
     * @return $data['status']   1成功  0失败
    */
    SnsApi::cApi('Vip/update',$info);
````

