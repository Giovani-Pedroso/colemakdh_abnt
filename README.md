# colemakdh_abnt
Add this lines to the end of the file: /usr/share/X11/xkb/symbols/br   

```
// The colemak to abnt2
//partial alphanumeric_keys
xkb_symbols "colemakbr" {

    include "br(abnt2)"
    name[Group1]="colemak";

    key <AD01> { [            q,              Q,         slash,           slash ] };
    key <AD02> { [            w,              W,      question,        question ] };
    key <AD03> { [            f,              F,        degree,          degree ] };
    key <AD04> { [            p,              P,    registered,      registered ] };
    key <AD05>	{ [         b,          B,       tslash,       Tslash ]	};
    key <AD06>	{ [         j,          J,    leftarrow,          yen ]	};
    key <AD07>	{ [         l,          L,    downarrow,      uparrow ]	};
    key <AD08>	{ [         u,          U,   rightarrow,     idotless ]	};
    key <AD09>	{ [         y,          Y,       oslash,       Oslash ]	};
    key <AD10>	{ [       semicolon,          colon, dead_belowdot,   dead_abovedot]	};

    key <AC01>	{ [         a,          A,           ae,           ae ]	};
    key <AC02>	{ [         r,          R,       ssharp,        u1e9e ]	};
    key <AC03>	{ [         s,          S,          eth,          eth ]	};
    key <AC04>	{ [         t,          T,      dstroke,  ordfeminine ]	};
    key <AC05>	{ [         g,          G,          eng,          eng ]	};
    key <AC06>	{ [         m,          M,      hstroke,      hstroke ]	};
    key <AC07>	{ [         n,          N,    dead_hook,    dead_horn ] };
    key <AC08>	{ [         e,          E,          kra,    ampersand ]	};
    key <AC09>	{ [         i,          I,      lstroke,      lstroke ]	};
    key <AC10> { [     o,       O,    dead_acute,dead_doubleacute ] };

    key <LSGT>	{ [         z,          Z, guillemotleft,        less ]	};
    //key <BKSL>	{ [         z,          z, guillemotleft,        less ]	};
    key <AB01>	{ [         x,          X, guillemotleft,        less ]	};
    key <AB02>	{ [         c,          C, guillemotright,    greater ]	};
    key <AB03>	{ [         d,          D,         cent,    copyright ]	};
    key <AB04>	{ [         v,          V,   doublelowquotemark, singlelowquotemark ]	};
    key <AB05>	{ [       ccedilla,       Ccedilla ,  leftdoublequotemark, leftsinglequotemark ] };
    key <AB06>	{ [         k,          K, rightdoublequotemark, rightsinglequotemark ]	};
    key <AB07>	{ [         h,          H,            mu,    masculine ]	};
    key <AB10>	{ [     slash,   question, dead_belowdot, dead_abovedot ] };
    key <AB11>	{ [    backslash,        bar,   dead_grave,   dead_breve ] };
};            
```

then run the command in the terminal:

```
setxkbmap -model abnt2 -layout br -variant colemakbr
```
