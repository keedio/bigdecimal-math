all: BigDecimalMath.jar Wigner3jGUI.jar html

#	- javadoc -Xdoclint:none -sourcepath . -private -d html org.nevec.rjm
html:
	- javadoc -sourcepath . -private -d html org.nevec.rjm

BigDecimalMath.jar:
	javac org/nevec/rjm/*.java
	jar cf $@ org

Wigner3jGUI.jar:
	javac org/nevec/rjm/*.java
	jar cmf Wigner3jGUI.mf $@ org/nevec/rjm/*.class

distclean:
	rm -rf html *.jar org/nevec/rjm/*.class
