from building import *
Import('rtconfig')

src   = []
cwd   = GetCurrentDir()

# add rx8010 src files.
if GetDepend('PKG_USING_RX8010'):
    src += Glob('src/rx8010.c')

# add rx8010 include path.
path  = [cwd + '/inc']

# add src and include to group.
group = DefineGroup('rx8010', src, depend = ['PKG_USING_RX8010'], CPPPATH = path)

Return('group')
