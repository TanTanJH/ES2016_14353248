# **Lab2���⣺�汾����&�ĵ�**
## **Description**
�ֲ�ʽ�����㣨DOL����һ�����벢��Ӧ�ó�������������ܣ�������ָ������Kahn�����������ģ�ͺ���SystemC��ģ������Ϊ��ɫ��Ӧ�á����⣬DOL���ṩ�˻���XML�Ĺ淶��ʽ�������ദ����ϵͳ�ϰ����󶨺�ӳ��Ĳ���Ӧ�ó����ʵ�֡�
## **How to install**
### ����
####1.ʹ���������װUbuntu
####2.��װ����
  a)sudo apt-get update
  b)sudo apt-get install ant
  c)sudo apt-get install openjdk-7-jdk
  d)sudo apt-get install unzip
####3.�����ļ�
  a)sudo wget http://www.accellera.org/images/downloads/standards/systemc/systemc-2.3.1.tgz
  b)sudo wget http://www.tik.ee.ethz.ch/~shapes/downloads/dol_ethz.zip
####4.��ѹ�ļ�
  a)mkdir dol���½�dol�ļ��У�
  b)unzip dol_ethz.zip -d dol����dolethz.zip��ѹ�� dol�ļ����У�
  c)tar -zxvf systemc-2.3.1.tgz����ѹsystemc��
####5.����systemc
  a)cd systemc-2.3.1������systemc-2.3.1��Ŀ¼��
  b)mkdir objdir���½���ʱ�ļ���objdir��
  c)cd objdir
  d)../configure CXX=g++ --disable-async-updates������configure��
  e)sudo make install�����룩
  f)cd ../dol
    �޸�build_zip.xml�ļ�
####6.����dol
  a)ant -f build_zip.xml all

## **Experimental experience**
  �ܵ���˵��DOL��������û��ʲô������⣬�����ڰ�װ������ֱ����ubuntu������վ���ص�ѹ�������ܳ����ļ��𻵵������������Դ�Լ����粻�ȶ����������ڵ�һ���������ʱ������ʾ�ļ�ȱʧ�����ֱ�����ⲿ������Ϻ��Ͻ��������ɺ������衣