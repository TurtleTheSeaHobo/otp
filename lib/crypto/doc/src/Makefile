# ``Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
#
# The Initial Developer of the Original Code is Ericsson Utvecklings AB.
# Portions created by Ericsson are Copyright 1999, Ericsson Utvecklings
# AB. All Rights Reserved.''
#
#     $Id$
#
include $(ERL_TOP)/make/target.mk
include $(ERL_TOP)/make/$(TARGET)/otp.mk

# ----------------------------------------------------
# Application version
# ----------------------------------------------------
include ../../vsn.mk
VSN=$(CRYPTO_VSN)
APPLICATION=crypto

# ----------------------------------------------------
# Target Specs
# ----------------------------------------------------
XML_APPLICATION_FILES = ref_man.xml
XML_REF3_FILES = crypto.xml
XML_REF6_FILES = crypto_app.xml

XML_PART_FILES = usersguide.xml
XML_CHAPTER_FILES = notes.xml licenses.xml fips.xml engine_load.xml engine_keys.xml \
	algorithm_details.xml new_api.xml

BOOK_FILES = book.xml

XML_FILES = $(BOOK_FILES) $(XML_APPLICATION_FILES) $(XML_REF3_FILES)  $(XML_REF6_FILES) \
            $(XML_PART_FILES) $(XML_CHAPTER_FILES)

IMAGE_FILES =

TOP_SPECS_FILE = specs.xml

include $(ERL_TOP)/make/doc.mk

valgrind asan:
