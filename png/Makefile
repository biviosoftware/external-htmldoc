#
# "$Id$"
#
#   PNG library Makefile for the HTMLDOC software.
#
#   Makefile copyright 1997-2001 by Easy Software Products, all rights reserved.
#   PNG library copyright 1995 Guy Eric Schalnat, Group 42, Inc.
#   For conditions of distribution and use, see copyright notice in png.h
#
#   These coded instructions, statements, and computer programs are the
#   property of Easy Software Products and are protected by Federal
#   copyright law.  Distribution and use rights are outlined in the file
#   "LICENSE.txt" which should have been included with this file.  If this
#   file is missing or damaged please contact Easy Software Products
#   at:
#
#       Attn: HTMLDOC Licensing Information
#       Easy Software Products
#       44141 Airport View Drive, Suite 204
#       Hollywood, Maryland 20636-3142 USA
#
#       Voice: (301) 373-9600
#       EMail: info@easysw.com
#         WWW: http://www.easysw.com
#

include ../Makedefs

#
# Object files...
#

OBJS	=	png.o pngset.o pngget.o pngrutil.o pngtrans.o pngwutil.o \
		pngread.o pngrio.o pngwio.o pngwrite.o pngrtran.o \
		pngwtran.o pngmem.o pngerror.o pngpread.o

#
# Make all of the targets...
#

all:	libpng.a

#
# Clean all of the targets and object files...
#

clean:
	$(RM) $(OBJS)
	$(RM) libpng.a

#
# libpng.a
#

libpng.a:	$(OBJS)
	echo Archiving $@...
	$(RM) $@
	$(AR) $(ARFLAGS) $@  $(OBJS)
	$(RANLIB) $@

$(OBJS):	png.h pngconf.h ../Makedefs

#
# End of "$Id$".
#
