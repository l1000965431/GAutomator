v 1.1.1 �汾������־��
====================
-----------------------------------
device=manager.get_device():
*�����ӿ�get_element_world_bound���ܹ���ȡ���ڵ���������ꡣ�÷���ֻ֧��wetest sdk 8�汾��������
*�����ӿ�get_registered_handlers����ȡ���õ��Զ��庯�����÷���ֻ֧��wetest sdk 8�汾��������
*�����ӿ�call_registered_handler����������Ϸ��ע����Զ��庯���������ض�Ӧ��ֵ���÷���ֻ֧��wetest sdk 8�汾��������
~�޸�:NGUI���ְ汾,����Input������

main.py:
*�����Ϸ����������main.py�ܹ�ֱ��������Ϸ��������ȫ�߼��Ĳ���

trave.py
*�����Զ���̽�����Խӿڣ����㲻д����Ҳ����ֱ�ӱ�����Ϸ


v 1.2.1 �汾������־
====================
-----------------------------------
engine=manager.get_engine():
*�����ӿ�get_touchable_elements_bound���ܹ���ȡ�ɵ���ڵ㼰�ڵ����Ͻ����꣬�ڵ㳤���
*�����ӿ�get_element_text,��ȡGameObject������Ϣ��NGUI�ؼ����ȡUILable��UIInput��GUIText����ϵ�������Ϣ��UGUI�ؼ����ȡText��GUIText����ϵ�������Ϣ
*�����ӿ�get_element_image,��ȡGameObjectͼƬ����,NGUI�ؼ����ȡUITexture��UISprite��SpriteRenderer����ϵ�ͼƬ����,UGUI�ؼ����ȡImage��RawImage��SpriteRenderer����ϵ�ͼƬ����

-----------------------------------
device=manager.get_device():
*get_display_size,�ƶ˻�ȡʧ�ܺ�ֱ��ͨ��uiautomator��ȡ������ֱ��ͨ��Uiautomator��ȡ
*get_rotation���ƶ˴�ƽ̨��ȡʧ�ܺ�ֱ��ͨ��UIAutomator��ȡ������ֱ��ͨ��UIAutomator��ȡ
*get_top_package_activity,�ƶ˴�ƽ̨��ȡʧ�ܺ�ֱ��ͨ��UIAutomator��ȡ������UIAutomator��ȡʧ�ܺ�ͨ��adb shell dumpsys��ȡ
*back�����ط�ʽ�޸�ΪUIAutomator

-----------------------------------
��½ʵ�ֽ������޸�
-----------------------------------
��uiautomator�����������Ա�����
-----------------------------------
main.py�޸ģ��޸�native����Ϸ����ʱ������������Ϸ���ٽ���socket�ĳ�ʼ��


v 2.0.0�汾
====================
V2�汾�����ټ����ϰ汾��SDK���µ�SDKҲ���ܼ����ϵĽű�GAutomator��ܡ�

V2�汾��Ҫ��GAutomator�Ŀ�ܽ����˸Ľ���ͨ��Э��ȫ����Ϊjson����python�İ汾Ҳû��windows 32��Ҫ���¼ܹ���֧����SDK�����������׼�ؼ��Ĳ���Ҳ�����ȶ���
SDK�����ܸ��Ӹ�Ч���Զ������Ի�����FPS��Ӱ��������Ժ��ԣ�CPU��Ӱ��һ����1%�����ҡ�
-----------------------------------
engine=manager.get_engine():
*����get_component_field,�ܹ������ȡ��Ϸ�ж��������ֵ

v 2.1.0�汾
====================
V2.1.0�汾��Ҫ�Կ�ܵĽṹ�����˵���

-----------------------------------
1��֧��һ̨pcͬʱ���ƶ�̨�ֻ�
2�����ڶ���ӿ��޹ص�wpyscripts.wetest.tools�Ƶ�wpyscripts.common.utils.py��wpyscripts.platform_helper.py�Ƶ�wpyscripts.common.platform_helper.py
3����logger_config.py�Ƴ�����־��ʼ�����õ�wpyscripts.__init__.py
4��get_touchable_elements_bound��get_touchable_element����Ĭ�ϵ�compnentΪ�ɵ����ѡ֮�⣬���������Զ����UI�ɵ���ؼ�������磬lua�ű���д������
5������component������ƻ�ȡgameobject

------------------------------------
GAutomatorView
1���޸�android 5.0����ͼƬ��ת������ʹ�õ�bug
2���޸��������ڴ�Сʱ����ɫ������ԭ�أ�λ�÷���ƫ�Ƶ�bug
3������gameobject�������Ĺ��ܣ�֧��������ʽ����
4������·�����ܽ��е�����2.0.0�汾����ʱ�Ḵ��ȫ·����2.1.0�汾���gameobject�����жϣ��������Ψһֻ�������ƣ�������Ʋ�Ψһ����ȫ·��
5���޸����ָ��ı�������<ʱ��֧�ֵ�bug


v 2.2.0�汾
====================

-----------------------------------
1��Ĭ�������ѡ��һ��������ܻᱻ����������Ⱦ����������һ����ǡ���������
2���޸�QQ��΢�������ǲ����ֻ����޷���½��BUG
3���Ƴ�runTest.sh��endTest.sh�������Ҫ��������end.py��prepare.py
4���޸�����Linux��Mac���ز������е�bug
5���޸�get_element_bound�����ɼ������ݷ���ElementBound��visible������Ϊfalse;��Ҫ���3D���壬ת��Ϊ��Ļ����ʱ���������Χ֮�����Ϊvisible=false
6������urllib3�⣬�����û���װ������urllib3��֮���ܹ�����������python����0���ã�һ�ݽű�������ֲ������ط���
7������linux�Ĳ��ԣ�������linux�¿�����

v 2.3.0 �汾
====================

------------------------------------
1�����ӻ�ȡ����Ϸ�����ִ�ж�Ӧ�����Ľӿڡ�
2���޸�����bug��


v 2.3.1���汾
====================

------------------------------------
1���޸�SDK�ڲ���unity�汾�ϣ���ȡӦ�ó���߲�׼��bug

V 2.4.0 �汾
=====================
1���޸��ű�������bug
2��report�ӿ�����report_error�ӿڣ��û����ܲ��ԵĶ��ԡ��ڱ������л�������Ŀ¼������_wetest_testcase_result.txt��ͳ����Ϣ


V 2.5.0 �汾
=====================
1���Ǽ����gameobject������get_element_bound���ص�visibleΪfalse
2���޸�����boxcolidr�����س��������bug
3������������C#�ű����ã��ɶ�̬��ȡ�������Ϸ�ڽӿ�


