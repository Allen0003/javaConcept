Annotation can tell JVM some information in advance 

1. 
Annotation ��{���B��S���v�T�A
�����ت��b��sĶ���Τ��R�u�㻡���{�����Y�Ǹ�T�A

such as @Override

2. 
�Хܪ���k�O�@�Ӥ���ĳ�Q�ϥΪ���k�A�p�G���}�o�H�����p�ߨϥΤF�Q 
@Deprecated �Хܪ���k�A�sĶ���n���Xĵ�T�����}�o�H���C

such as 

�@�ǳQ������code and still can work very well 

3. 
�ۭq Annotation ���A

��z�ϥ� @interface �ۦ�w�q Annotation ���A�ɡA
��ڤW�O**�۰��~��**�F java.lang.annotation.Annotation �����A

i.public @interface BackstageLogAction {

ii.
public @interface UnitTest {
	String value();
}

��ڤW�z�w�q�F value() ��k�A�sĶ���b�sĶ�ɷ|�۰����z���ͤ@�� 
value ����Ʀ����A���ۦb�ϥ� UnitTest Annotation �ɭn���w�ȡA�Ҧp�G

public class MathTool {
    @UnitTest("GCD")
    public static int gcdOf(int num1, int num2) {
		// ....
    }
}
@UnitTest("GCD") ��ڤW�O @UnitTest(value="GCD) 

�O�o�ϥ� import �i�D�sĶ�����A���M���m�A�Ҧp�G

import onlyfun.caterpillar.Debug;

�A�ӭn���ovalue �򤧫e�����O�M�b�@�_�N�n