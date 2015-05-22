include ../Makefile.inc

# for now this list needs to be sync'ed manually with make_release.sh

APPS = read_label kmerPrefixCounter make_db_table tax_histo rand_read_label content_summ gene_label frequency_counter

OBJECTS = $(addsuffix .o,$(APPS))
DATA = $(METAG_DIR)/dev/src/kmerdb/examples/tests/data


all: $(APPS)


clean: 
	$(RM) $(OBJECTS) $(APPS)



read_label: $(METAG_LIB) read_label.cpp
	$(CXX) -std=c++0x $(CXXFLAGS) $(LDFLAGS) $@.cpp $(LIBS) -o $@
	cp read_label ../bin


kmerPrefixCounter: $(METAG_LIB) kmerPrefixCounter.cpp
	$(CXX) -std=c++0x $(CXXFLAGS) $(LDFLAGS) $@.cpp $(LIBS) -o $@
	cp kmerPrefixCounter ../bin


make_db_table: $(METAG_LIB) make_db_table.cpp
	$(CXX) -std=c++0x $(CXXFLAGS) $(LDFLAGS) $@.cpp $(LIBS) -o $@
	cp make_db_table ../bin


tax_histo: $(METAG_LIB) tax_histo.cpp
	$(CXX) -std=c++0x $(CXXFLAGS) $(LDFLAGS) $@.cpp $(LIBS) -o $@
	cp tax_histo ../bin


rand_read_label: $(METAG_LIB) rand_read_label.cpp
	$(CXX) -std=c++0x $(CXXFLAGS) $(LDFLAGS) $@.cpp $(LIBS) -o $@
	cp rand_read_label ../bin


content_summ: $(METAG_LIB) content_summ.cpp
	$(CXX) -std=c++0x $(CXXFLAGS) $(LDFLAGS) $@.cpp $(LIBS) -o $@
	cp content_summ ../bin


gene_label: $(METAG_LIB) gene_label.cpp
	$(CXX) -std=c++0x $(CXXFLAGS) $(LDFLAGS) $@.cpp $(LIBS) -o $@
	cp gene_label ../bin


frequency_counter: $(METAG_LIB) frequency_counter.cpp
	$(CXX) -std=c++0x $(CXXFLAGS) $(LDFLAGS) $@.cpp $(LIBS) -o $@
	cp frequency_counter ../bin


