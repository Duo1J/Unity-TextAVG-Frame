Duo1J AVG Frame Demo~

����Hierarchy���������������AVG Frame�ű�

AVGFrame.cs-------------------
Image Url Prefix: ͼ���ļ�·��ǰ׺�� ��Resources�ļ����д��ͼ���ļ���ǰ׺
Audio Url Prefix: ͬ��
TextAsset: ��AVGFrame�е��ݳ��ű�

UI Component-----
Canvas: ����UI�������
Text: �Ի���ʾText���
Name Text: ��ɫ������ʾText���
Character Image: ��ɫ������ʾImage���
Background Image: ����ͼƬ��ʾImage���
Character Voice: ��ɫ����Audio Source���
Background Music: ��������Audio Source���

----------------------------------------------------------------------------------------------------------------
�ݳ��ű���д��ʽ��
�ַ�Ҫ��UTF-8

�������  demo.txt

ע��: #
�ű��еĿ�����Ҫ#ռλ

�ı�ָ��: T/��ɫ��/�Ի��ı�/����/�ӳ�����:�ӳ�ʱ��/.../ (������)
����: T/Jack/Hello/Jack01.mp3/2:0.5/   (�ڲ��ŵ�eʱ���ӳ�0.5s)
��ɫ���������̳���һ������֣������ʹ��C���������������ı�
������Ҫ�����ӳ�,��: T/Ketty/12345//2:0.5/3:0.5/4:0.5/ �ɸĳ� => T/Ketty/12 3 45//2:0.5/4:0.5/6:0.5/

ϵͳָ��: C/��ɫimg/imgλ��/xƫ��/yƫ��/����img/����audio/
����: C/p01/0/0/80/bk2/ϫ.mp3/
x,yƫ��Ĭ��Ϊ0����������
imgλ��ֻ������0 1 2,  0-����1-���У�2-����
ֻ��audio���������ļ���׺

ѡ��ťָ��: B/�¼�����/ѡ��1/ѡ��2/.../ (������)
����: B/Event01/Study/Shop

����ָ��: A/��������/
�������Ͳ����ִ�Сд
�Դ�����: 'ch_shake'��ɫ�ζ� 'bk_shake'�����ζ�
����: A/ch_shake/
�Զ��嶯������дDuo1JAnimation�ӿڲ�������AVG Frameͬһ����

����ָ����/��β�� ��ĳ����������Ҫ��//����
����: T/Mary/Goodbye!///  �������ӳپ���ʹ��

ͼƬ�ļ����Ӻ�׺����Ƶ�ļ��Ӻ�׺

interface----------------------------------------------------------------------------------------------------
����ʵ���˽ӿں��������AVGFrameͬ�����ϼ���,�ɲο�InterfaceExample.cs

Duo1JAround�ӿ�-----------------------------------------
ʵ��void After()��void Before()����
Before()��After()�ڲ��ŵĿ�ʼ�ͽ���ʱ�����

Duo1JAnimation�ӿ�-----------------------------------------
ʵ��void StartAnimation(string type)����
typeΪ A/type/ ָ���е�type

Duo1JAction�ӿ�--------------------------------------------
ʵ��void GetButtonChoose(string eventTag, Choose choose)����
eventTagΪ B/event/choose1/choose2/.../ָ���е�event
Choose.index��Choose.textΪѡ�������������

Duo1JLoader�ӿ�-------------------------------------
ʵ��bool Analysis(out List<AVGModel> modelList, UnityEngine.TextAsset textAsset)����
����ֵΪ�Ƿ�����ɹ�
����textAsset��AVGModel���󣬷��ص�modelList��

Duo1JInput�ӿ�---------------------------------------
ʵ��bool Input_Next()����
������������Ƿ񲥷���һ��