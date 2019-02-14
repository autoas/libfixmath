from building import *

cwd = GetCurrentDir()

Import('asenv')
MODULES = asenv['MODULES']

objs = []

objs += Glob('libfixmath/*.c')
objs += Glob('contrib/*.c')

asenv.Append(CPPPATH=['%s/libfixmath'%(cwd)])
asenv.Append(CPPDEFINES=['FIXMATH_SIN_LUT','FIXMATH_NO_CACHE'])

Return('objs')
